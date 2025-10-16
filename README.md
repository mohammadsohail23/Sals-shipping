# Sal’s Shipping 🚚

A Python 3 project from Codecademy’s *Learn Python 3* course that calculates the most affordable shipping method for a given package weight using **Sal’s Shippers**.

---

## 👨‍💻 Author
**Mohammad Z. Sohail**

---

## 🧾 Description
This program determines the cost of shipping based on three options:

1. **Ground Shipping** – A flat rate of \$20 plus a price per pound.  
2. **Ground Shipping Premium** – A flat rate of \$125, no weight charge.  
3. **Drone Shipping** – Higher rates per pound but no flat charge.

It demonstrates conditional statements (`if`, `elif`, `else`) and logical comparison to determine costs.

---

## 🐍 Code Example
```python

weight = 80

# Ground Shipping 🚚
if weight <= 2:
  cost_ground = weight * 1.5 + 20
elif weight <= 6:
  cost_ground = weight * 3.00 + 20
elif weight <= 10:
  cost_ground = weight * 4.00 + 20
else:
  cost_ground = weight * 4.75 + 20

print("Ground Shipping $", cost_ground)
      
# Ground Shipping Premium 🚚💨
cost_ground_premium = 125.00
print("Ground Shipping Premium $", cost_ground_premium)

# Drone Shipping 🛸
if weight <= 2:
  cost_drone = weight * 4.5
elif weight <= 6:
  cost_drone = weight * 9.00
elif weight <= 10:
  cost_drone = weight * 12.00
else:
  cost_drone = weight * 14.25

print("Drone Shipping: $", cost_drone)
