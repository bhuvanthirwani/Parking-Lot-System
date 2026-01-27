# 🅿️ Parking Lot System

> **A Command-Line Interface for Parking Management**

This project simulates a **Parking Lot Management System**. It provides a robust command-line interface to manage parking slots, park cars, and handling vehicle departures efficiently. It also offers advanced querying capabilities based on driver age and vehicle registration numbers.

---

## 🛠 Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Language** | ![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat&logo=python&logoColor=white) |
| **Input/Output** | File I/O (`input.txt`) / Standard Output |

---

## 🚀 Key Features

-   **🅿️ Dynamic Parking Lot Creation**: Initialize a parking lot with a user-defined capacity.
-   **🚗 Park Vehicle**: Automatically assigns the nearest available slot to an incoming vehicle.
-   **👋 Leave & Vacate**: Handles vehicle departure and frees up the slot.
-   **🔍 Advanced Queries**:
    -   Find slot number by vehicle registration number.
    -   Find slot numbers for all drivers of a specific age.
    -   Find vehicle registration numbers for all drivers of a specific age.

---

## 📖 Supported Commands

The system reads commands from `input.txt`. Below are the supported operations:

| Command | Description | Example |
| :--- | :--- | :--- |
| `Create_parking_lot` | Creates a parking lot of size `n` | `Create_parking_lot 6` |
| `Park` | Parks a car with vehicle number and driver age | `Park KA-01-HH-1234 driver_age 21` |
| `Slot_numbers_for...` | Finds slots for a given driver age | `Slot_numbers_for_driver_of_age 21` |
| `Slot_number_for...` | Finds slot of a specific car | `Slot_number_for_car_with_number KA-01-HH-1234` |
| `Leave` | Vacates a specific slot number | `Leave 2` |
| `Vehicle_registration...` | Finds reg numbers by driver age | `Vehicle_registration_number_for_driver_of_age 21` |

---

## 📦 How to Run

1.  **Clone the repository**
    ```bash
    git clone https://github.com/yourusername/Parking-Lot-System.git
    cd Parking-Lot-System
    ```

2.  **Prepare Input File**
    Modify `input.txt` with your desired commands.

3.  **Run the application**
    ```bash
    python main.py
    ```

4.  **View Output**
    The system will process the commands and print the output to the console.

---

## 📝 Example `input.txt`

```text
Create_parking_lot 6
Park KA-01-HH-1234 driver_age 21
Park PB-01-HH-1234 driver_age 21
Slot_numbers_for_driver_of_age 21
Park PB-01-TG-2341 driver_age 40
Slot_number_for_car_with_number PB-01-HH-1234
Leave 2
```

---

*Efficient parking management simplified.*