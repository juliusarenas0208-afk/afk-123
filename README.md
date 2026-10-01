Students = int(input("Students: "))

def Student_info():
    name = input("Enter name: ")
    ACT_1 = float(input("Activity 1:"))
    ACT_2 = float(input("Activity 2:"))
    ACT_3 = float(input("Activity 3:"))

    average = (ACT_1 + ACT_2 + ACT_3) / 3
    return average

def Status_ave(average):
    if average >= 90:
        return "Excellent"

    elif average >= 80:
        return "Very Good"

    elif average >= 75:
        return "Passed"

    else:
        return "Failed"

for i in range (Students):
    print("Students", i + 1)

    average = Student_info()
    status = Status_ave(average)

print("\n__Student Result__")
print("Average:", round(average, 2))
print("Status:", status)
