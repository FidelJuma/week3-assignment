
# week3-assignmentCreate a function named calculate_discount(price, discount_percent) that calculates the final price after applying a discount. The function should take the original price (price) and the discount percentage (discount_percent) as parameters. If the discount is 20% or higher, apply the discount; otherwise, return the original price.
Using the calculate_discount function, prompt the user to enter the original price of an item and the discount percentage. Print the final price after applying the discount, or if no discount was applied, print the original price.
Here's a Python code that defines the `calculate_discount` function and prompts the user to enter the original price and discount percentage:

```python
def calculate_discount(price, discount_percent):
    # Check if the discount is 20% or higher
    if discount_percent >= 20:
        discount_amount = price * (discount_percent / 100)
        final_price = price - discount_amount
        return final_price
    else:
        return price

# Prompt the user for input
price = float(input("Enter the original price of the item: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate the final price
final_price = calculate_discount(price, discount_percent)

# Print the result
if final_price == price:
    print(f"No discount applied. The original price is: ${price:.2f}")
else:
    print(f"The final price after applying the discount is: ${final_price:.2f}")
```

### How it works:
1. The function `calculate_discount(price, discount_percent)` checks if the discount percentage is 20% or higher.
2. If the condition is met, it calculates the discount amount and subtracts it from the original price to get the final price.
3. If the discount is less than 20%, the original price is returned without any changes.
4. The program then prompts the user to input the original price and discount percentage.
5. Finally, it prints either the discounted price or the original price depending on whether the discount was applied.

Let me know if you'd like me to explain or modify anything!
