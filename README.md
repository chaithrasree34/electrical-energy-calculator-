# Electrical Energy Calculator

print("ELECTRICAL ENERGY CALCULATOR")
print("----------------------------")

# Input values
power = float(input("Enter appliance power (W): "))
hours = float(input("Enter usage time per day (hours): "))
days = int(input("Enter number of days: "))
tariff = float(input("Enter electricity tariff (₹ per kWh): "))

# Energy calculation
energy_kwh = (power * hours * days) / 1000

# Cost calculation
cost = energy_kwh * tariff

# Average daily energy
daily_energy = (power * hours) / 1000

# Display results
print("\n--- Results ---")
print(f"Daily Energy Consumption = {daily_energy:.2f} kWh")
print(f"Total Energy Consumption = {energy_kwh:.2f} kWh")
print(f"Electricity Cost         = ₹{cost:.2f}")# electrical-energy-calculator-