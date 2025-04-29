---
title: "Python Mini Project"
date: 2025-11-15T15:34:30-04:00
categories:
  - code
tags:
  - programming
  - CSS
---

```
import matplotlib.pyplot as plt
expenses = []
def add_expense():
    date = input("Enter the date (YYYY-MM-DD): ")
    category = input("Enter the category (e.g., groceries, entertainment, utilities): ")
    amount = input("Enter the amount: ")
    expenses.append({"date": date, "category": category, "amount": float(amount)})
    print("Expense added successfully!")
def show_summary():
    if len(expenses) == 0:
        print("No expenses to summarize.")
        return
    total = sum(expense['amount'] for expense in expenses)
    print(f"Total spending: ${total:.2f}")
    categories = {}
    for expense in expenses:
        if expense['category'] in categories:
            categories[expense['category']] += expense['amount']
        else:
            categories[expense['category']] = expense['amount']
    print("Spending by category:")
    for category, amount in categories.items():
        print(f"{category}: ${amount:.2f}")
def visualize_data():
    if len(expenses) == 0:
        print("No expenses to visualize.")
        return
    categories = {}
    for expense in expenses:
        if expense['category'] in categories:
            categories[expense['category']] += expense['amount']
        else:
            categories[expense['category']] = expense['amount']
    plt.bar(categories.keys(), categories.values())
    plt.title("Spending by Category")
    plt.xlabel("Category")
    plt.ylabel("Amount")
    plt.show()

    print("Personal Expense Tracker")
    print("1. Add an Expense")
    print("2. Show Summary Report")
    print("3. Visualize Data")
    print("4. Exit")
    choice = input("Choose an option: ")
    if choice == "1":
        add_expense()
    elif choice == "2":
        show_summary()
    elif choice == "3":
        visualize_data()
    elif choice == "4":
        print("Goodbye!")

    else:
        print("Invalid choice. Please try again.")
```