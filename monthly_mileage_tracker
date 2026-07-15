## month and miles arrays for code.
MonthArray = []
MilesDriven = []


# function to populate arrays
def PopulateArray():
    position = 0

    # This loop collects five names and appends them to the namelist
    while (position < 12):

        # append each array
        monthname = input("Please enter a month name:\n")
        MonthArray.append(monthname)

        totalmiles = input("Please enter miles driven for the month:\n")
        MilesDriven.append(totalmiles)

        # counts position +1 while in the loop of 12
        position = position + 1

    return


# function to find month.
def searchformonth(monthtosearch):
    foundposition = -1  # assume that it is not going to be found.
    position = 0

    # while in loop of 12
    while (position < 12):

        if (monthtosearch == MilesDriven[position]):
            foundposition = position

            # prints exact month and miles driven depending on the user
            print("The month name is:" + MonthArray[position] +
                  "and the miles driven for the month is: " +
                  str(MilesDriven[position]))

            break

        position = position + 1

    # returns
    return foundposition


# This function displays the menu, collects the user response and sends it back.
def displaymenu():
    print("**** MENU OPTIONS ****")
    print("Type P to populate miles and month name.")
    print("Type S to search for Month")
    print("Type M to search for Month name with smallest Miles")
    print("Type L to search for Month Name with Largest Miles")
    print("Type E to exit")

    choice = input("Please enter your choice:\n")
    return choice


# main choice
choice = displaymenu()

# while condition not equal to !=
while (choice != ""):

    # if condition when the user chooses
    if (choice == "P"):
        PopulateArray()

    # elif (choice=="S"):
    # monthtofind = input("Please enter the month name to search:\n")

    # Program exits when user types E.
    elif (choice == "E"):
        print("Thank you for using the program.")
        print("Bye")
        break

    # else if user types option not on menu.
    else:
        print("Invalid choice. Please try again!")

    # displays menu again after user is finished with their choice.
    choice = displaymenu()
