
# Final Project
# Service Price Calculator with Add-Ons

# Dictionary containing services and prices
services = {
    "Clear Skin Facial": 75.00,
    "Hydration Facial": 100.00,
    "Brow Lamination": 60.00,
    "Wax Me Pretty": 80.00,
    "Glow Wax": 55.00,
}

# Dictionary containing add-ons and prices
addons = {
    "Jelly Mask": 10.00,
    "Extractions": 5.00,
    "Massage": 25.00,
}


# Function to display the main menu
def menu():

    print("\n=== PRICE CALCULATOR ===")
    print("1. View Services")
    print("2. View Add-Ons")
    print("3. Calculate Appointment Price")
    print("4. Exit")

    choice = input("Enter your choice: ")

    return choice

# Function to display services
def view_services():

    print("\n=== SERVICES ===")

    for name, price in services.items():
        print(name, "- $", format(price, ".2f"))

# Function to display available add-ons
def view_addons():

    print("\n=== ADD-ONS ===")

    for name, price in addons.items():
        print(name, "- $", format(price, ".2f"))


# Function to calculate appointment price
def calculate_price():

    # Display services
    view_services()

    # Ask user to select a service
    service = input("\nEnter service name: ")

    # Check if service exists
    if service in services:

        # Get base service price
        total = services[service]

        print("\nBase Service:", service)
        print("Base Price: $", format(total, ".2f"))

        # Display add-ons
        view_addons()

        # Allow user to select add-ons
        while True:

            addon = input(
                "\nEnter add-on name or type Done: "
            )

            # Stop adding services
            if addon.lower() == "done":
                break

            # Check if add-on exists
            if addon in addons:

                # Add price to total
                total = total + addons[addon]

                print("Add-on added:", addon)

            else:

                print("Invalid.")

        # Display appointment total
        print("\n=== APPOINTMENT TOTAL ===")
        print("Service:", service)
        print("Total Price: $", format(total, ".2f"))

    else:

        print("Service not found.")

# Main function controls the application
def main():

    while True:

        choice = menu()

        if choice == "1":
            view_services()

        elif choice == "2":
            view_addons()

        elif choice == "3":
            calculate_price()

        elif choice == "4":
            print("Thank you for booking your appointment!")
            break

        else:
            print("Invalid choice.")


# Start the application
main()
