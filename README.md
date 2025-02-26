![CNC Plotter] 

## **Overview**  
This project is a **CNC 2D Drawing Machine** built using an **Arduino Uno**, **L293D motor driver**, and **two DVD-ROM stepper motors**. It is designed to draw vector-based graphics using **Inkscape** for G-code generation and **Processing** to send commands to the Arduino.  

## **Features**  
- Uses two **DVD-ROM stepper motors** for X and Y-axis movement.  
- A **micro servo motor** for pen lifting and placement.  
- Converts vector images to **G-code** using **Inkscape**.  
- Sends G-code commands to Arduino using **Processing software**.  

## **Components Used**  
| Component            | Quantity |
|----------------------|----------|
| Arduino Uno         | 1        |
| L293D Motor Driver Shield | 1 |
| DVD-ROM Stepper Motors | 2 |
| Micro Servo Motor   | 1 |
| Power Supply (12V)  | 1 |
| Drawing Pen         | 1 |
| Frame (custom-built) | 1 |

## **Circuit Diagram**  


## **Connections**  
| Arduino Pins | L293D Motor Shield |
|-------------|----------------------|
| X-axis Stepper | Motor 1 (M1, M2) |
| Y-axis Stepper | Motor 2 (M3, M4) |
| Servo Motor (Pen Lift) | Digital Pin 9 |

## **Software Setup**  

### **1. Generate G-code using Inkscape**  
1. Install **Inkscape** from [Inkscape.org](https://inkscape.org/).  
2. Install the **G-code extension** for Inkscape (such as **J Tech Photonics Plugin**).  
3. Open an image or create a drawing in Inkscape.  
4. Convert the drawing to a **path** (Path → Object to Path).  
5. Save the file as **G-code (.gcode or .nc format)**.  

### **2. Send G-code using Processing**  
1. Install **Processing** from [Processing.org](https://processing.org/).  
2. Load a Processing sketch that reads G-code and sends commands to Arduino via serial.  
3. Connect the Arduino to your PC and upload the **GRBL-based firmware**.  
4. Run the Processing script to start drawing.  

## **How It Works**  
- The **G-code file** generated by Inkscape contains movement instructions.  
- Processing reads the G-code and sends commands to the **Arduino Uno**.  
- The **stepper motors** move the pen in **X and Y directions** accordingly.  
- The **servo motor** lifts and places the pen based on the drawing path.  

## **Project Demo**  
  

## **Future Improvements**  
- Implement **Bluetooth/Wi-Fi control** using ESP8266 or ESP32.  
- Improve **drawing accuracy** with better motor drivers (e.g., A4988, DRV8825).  
- Enable **real-time image-to-G-code conversion** within Processing.

- Feel free to **fork this project, submit pull requests, or report issues**!
- ## **License**  
This project is open-source under the **MIT License**.  
-  

## **Contributing**  ![WhatsApp Image 2025-02-25 at 23 15 55_326f6c35](https://github.com/user-attachments/assets/459c92bd-1974-40c0-973a-41e8593668c7)

