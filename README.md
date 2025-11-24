# app.py

# Task 6: Add comments to explain the program's purpose and sections
"""
Weekly Study Time Calculator
This program takes daily study hours as input, estimates the total weekly study time, 
and includes basic error handling for non-numeric input.
"""

# Task 1: Add initial welcome message
print("Welcome to the Weekly Study Time Calculator!")

# --- Main Program Logic ---

# Task 5: Use a try/except block for robust input handling
try:
    # Task 2: Ask the user for input
    hours_input = input("\nEnter the number of hours you studied today: ")
    
    # Task 3: Convert Input (float) & Perform Calculations
    hours_studied_daily = float(hours_input)
    
    # Calculation 1: Estimate weekly hours (assuming 7 days of consistency)
    weekly_hours_estimate = hours_studied_daily * 7
    
    # Calculation 2: Calculate minutes studied today
    minutes_studied_today = hours_studied_daily * 60

    # Task 4: Display the Result Clearly
    print("\n--- Results ---")
    # Task 6: Use formatting for better readability (e.g., .2f for hours, .0f for minutes)
    print(f"Daily Study Time: {hours_studied_daily:.2f} hours ({minutes_studied_today:.0f} minutes)")
    print(f"Based on this, you are on track to study {weekly_hours_estimate:.2f} hours this week.")
    print("Keep up the great work!")

# Task 5 (Cont.): Handle the case where conversion to float fails
except ValueError:
    print("\n[ERROR] Please enter a valid numerical value for hours studied.")
    # Exit the program gracefully on error
    exit()

# Task 6: Check for and remove unused variables or test code (None found in this final version).
