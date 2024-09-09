# Display the welcome message to the user
print("Welcome to Package Express. Please follow the instructions below.")

# Prompt the user to enter the package weight
weight = float(input("Please enter the package weight: "))

# Check if the package weight is greater than 50
if weight > 50:
    # Display an error message if the package is too heavy
    print("Package too heavy to be shipped via Package Express. Have a good day.")
else:
    # Prompt the user to enter the package width
    width = float(input("Please enter the package width: "))
    
    # Prompt the user to enter the package height
    height = float(input("Please enter the package height: "))
    
    # Prompt the user to enter the package length
    length = float(input("Please enter the package length: "))
    
    # Check if the total dimensions exceed 50
    if width + height + length > 50:
        # Display an error message if the package is too big
        print("Package too big to be shipped via Package Express.")
    else:
        # Calculate the quote by multiplying the dimensions and weight, then dividing by 100
        quote = (width * height * length * weight) / 100
        
        # Display the calculated quote as a dollar amount
        print(f"Your estimated total for shipping this package is: ${quote:.2f}")
        print("Thank you!")
