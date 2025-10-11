# Ball-Balancing-Robot
Ball Balancing Robot – STM32F446 + PID Control + 3D Printed Mechanism
*Overview*
This project demonstrates a two-axis ball balancing robot built using an STM32F446 microcontroller and a PID feedback controller.
The system maintains the balance of a steel or plastic ball on a 3D-printed tilting platform by continuously adjusting servo motor angles based on real-time image data received from a camera module via UART communication.

⚙️ System Description:
The robot detects the ball’s position (X, Y) using a camera module, which transmits position data to the STM32F446 through the UART interface.
The controller then calculates the positional error relative to the center.
The PID controller implemented on the STM32F446 computes correction signals, which are output as PWM signals to two servo motors controlling the X and Y axes of the platform.
This creates a smooth and stable feedback loop to keep the ball centered.

🔁 Control Flow:
Capture real-time X and Y coordinates of the ball (via UART).
Error Calculation → Compute the deviation from the center (setpoint).
PID Control → Apply

<img width="468" height="88" alt="image" src="https://github.com/user-attachments/assets/8ed98639-6e4d-426a-92a4-2e4a88566fdf" />

Servo Control → Convert control output into PWM duty cycle signals for servos.
Feedback Update → Repeat continuously for real-time balance.

🚀 Features:
Dual-axis PID feedback stabilization
Real-time ball position control and display
UART-based camera communication for position tracking
Modular 3D-printed frame with servo mounts
Smooth motion response with low steady-state error

🎯 Project Goal:
To design and implement a real-time embedded control system using STM32F446 that demonstrates dynamic stability, mechanical design, and control theory through a fully 3D-printed mechatronic platform.



