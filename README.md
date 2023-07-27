# nimesa
import random

# Function to get weather data from the API (Replace this with actual API calls)
def get_weather_data():
    # Mock data for demonstration purposes
    temperature = random.randint(15, 35)
    humidity = random.randint(30, 80)
    return temperature, humidity

# Function to get wind speed data from the API (Replace this with actual API calls)
def get_wind_speed_data():
    # Mock data for demonstration purposes
    wind_speed = random.randint(0, 30)
    return wind_speed

# Function to get pressure data from the API (Replace this with actual API calls)
def get_pressure_data():
    # Mock data for demonstration purposes
    pressure = random.randint(980, 1050)
    return pressure

def main():
    while True:
        print("\nMenu:")
        print("1. Get weather")
        print("2. Get Wind Speed")
        print("3. Get Pressure")
        print("0. Exit")

        choice = int(input("Enter your choice: "))

        if choice == 1:
            temperature, humidity = get_weather_data()
            print(f"Weather: Temperature={temperature}°C, Humidity={humidity}%")
        elif choice == 2:
            wind_speed = get_wind_speed_data()
            print(f"Wind Speed: {wind_speed} km/h")
        elif choice == 3:
            pressure = get_pressure_data()
            print(f"Pressure: {pressure} hPa")
        elif choice == 0:
            print("Exiting the program.")
            break
        else:
            print("Invalid choice. Please choose again.")

if __name__ == "__main__":
    main()
