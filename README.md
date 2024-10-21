# HW_6.2


def convert_seconds(seconds):
    days = seconds // (24 * 60 * 60)
    seconds %= 24 * 60 * 60

    hours = seconds // (60 * 60)
    seconds %= 60 * 60

    minutes = seconds // 60
    seconds %= 60

    return f"{days} днів, {str(hours).zfill(2)}:{str(minutes).zfill(2)}:{str(seconds).zfill(2)}"

print(convert_seconds(0))        # 0 днів, 00:00:00
print(convert_seconds(224930))   # 2 днів, 14:28:50
print(convert_seconds(466289))   # 5 днів, 09:31:29
print(convert_seconds(950400))   # 11 днів, 00:00:00
print(convert_seconds(1296000))  # 14 днів, 00:00:00
print(convert_seconds(8639999))  # 99 днів, 23:59:59
print(convert_seconds(7948799))  # 91 днів, 23:59:59
