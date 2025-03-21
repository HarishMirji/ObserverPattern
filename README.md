# Observer Pattern for Weather Monitoring System

## Problem Statement
You are developing a weather monitoring system that collects data from various sensors such as temperature, humidity, and pressure sensors. When any sensor reading goes beyond a predefined threshold, you need to notify different weather stations through various communication channels like **emails, SMS, and push notifications**. Your task is to implement the **Observer pattern** to create a flexible notification system for this weather monitoring system.

## Assignment
Your goal is to implement the Observer pattern to refactor the existing `WeatherMonitoringApplication` class. The current class handles weather condition updates and notifications. Observer classes (e.g., `TemperatureService`, `PressureService`, `HumidityService`) need to be notified when any of the weather readings go beyond their respective thresholds.

## Implementing the Observer Pattern

### 1. Review the Original Class
- Study the `WeatherMonitoringApplication` class and its dependencies.
- Understand how it currently handles weather condition updates and notifications.

### 2. Implement the Publisher Class
- You have been provided with a `Publisher` abstract class.
- Implement the required methods defined by this interface in the `WeatherMonitoringApplication` class.
- Ensure the `Publisher` interface defines the methods necessary to notify observers.

### 3. Implement the Observer Interface
- Create an interface named `Observer`.
- This interface should include a method that takes weather conditions (e.g., temperature, humidity, pressure) as arguments.
- Observer classes (`TemperatureService`, `PressureService`, `HumidityService`) will implement this interface to receive notifications.

### 4. Refactor the Publisher
- Modify the `WeatherMonitoringApplication` class to adhere to the **Observer pattern**.
- **Do not change the constructor signature** as it's used by the tests.

### 5. Refactor the Observers
- Update the observer classes to implement the `Observer` interface.
- Modify their existing methods to match the new interface method signature.

### 6. Test Your Implementation
- Run the provided test cases in the `WeatherMonitoringTests` class.
- Verify that observers are notified appropriately.
- Ensure that the `WeatherMonitoringApplication` functions as expected.

## Instructions
1. Implement the **Observer pattern** by completing the `Publisher` and `Observer` interfaces.
2. Modify the observer classes (`TemperatureService`, `PressureService`, `HumidityService`) and the `WeatherMonitoringApplication` class accordingly.
3. Run the provided test cases in the `WeatherMonitoringTests` class to verify the correctness of your Observer pattern implementation.

