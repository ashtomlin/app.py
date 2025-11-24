# app.py
repository assignment 1
# app.py

# Task 1: Add initial welcome message
print("Welcome to the Weekly Study Time Calculator!")

# --- Main Program Logic ---

# Task 5: Add basic error handling using try/except
try:
    # Task 2: Ask the user for input
    # The theme chosen is 'Study Hours'.
    hours_input = input("\nEnter the number of hours you studied today: ")
    
    # Task 3: Convert Input & Perform a Calculation
    hours_studied_daily = float(hours_input)
    
    # Calculation: Estimate weekly hours
    weekly_hours_estimate = hours_studied_daily * 7
    
    # Calculation: Calculate minutes studied today (for a second small calculation)
    minutes_studied_today = hours_studied_daily * 60

    # Task 4: Display the Result Clearly
    print("\n--- Results ---")
    print(f"Daily Study Time: {hours_studied_daily:.2f} hours ({minutes_studied_today:.0f} minutes)")
    print(f"Based on this, you are on track to study {weekly_hours_estimate:.2f} hours this week.")
    print("Keep up the great work!")

# Handle the case where conversion to float fails
except ValueError:
    print("\n[ERROR] Please enter a valid numerical value for hours studied.")
    # Task 5: Use exit() after handling the error
    exit()

# Task 6: Final Cleanup & Comments (Comments added throughout)
# Note: No unused variables or test code were found in this final draft.
