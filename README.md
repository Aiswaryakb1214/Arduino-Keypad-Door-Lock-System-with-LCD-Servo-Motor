# Arduino-Keypad-Door-Lock-System-with-LCD-Servo-Motor

This project is an **Arduino-based electronic door lock system** that uses a **4x4 keypad** for password entry, an **LCD display** for user feedback, and a **servo motor** to lock/unlock the door.  

The system enhances security by requiring the correct password before granting access.  
It can be implemented in homes, offices, and restricted areas as a low-cost smart lock solution.  

---

## ✨ Features
- Secure access with **password verification**.
- **4x4 Keypad** for entering password input.
- **16x2 LCD Display** shows system status:
  - *Correct Password → Door Unlocked*
  - *Wrong Password → Access Denied*
- **Servo Motor** acts as the door lock/unlock mechanism.
- Automatically re-locks after a short delay.

---

## 🛠️ Components Required
- Arduino Uno
- 4x4 Keypad
- Servo Motor (SG90 / MG90)
- 16x2 I2C LCD Display
- Jumper wires, Breadboard, Power supply

---

## 📜 How it Works
1. User enters a password using the **keypad**.
2. When the `*` key is pressed:
   - If the entered password matches the predefined password:
     - LCD shows **“Correct Password – Door Unlocked”**
     - Servo motor rotates to 90° → Door unlocked
     - After a delay, the servo rotates back to 0° → Door locked
     - LCD shows **“Door Locked”**
   - If the entered password is incorrect:
     - LCD displays **“Wrong Password”**
     - Servo remains in locked position (0°).
3. The system then resets and waits for the next password entry.

---

## 📂 Project Structure
