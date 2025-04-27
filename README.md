# -DingDong-Done-Test-Doorbell-Counter-Track 

Here’s a demo of the project:

[Click to view the Video of Project Demo](https://youtu.be/9KLM3eui5tk)


Hello Technocratz! We proudly present the Smart Doorbell with LCD Counter and Click History.

The Smart Doorbell with LCD Counter and Click History is an innovative solution aimed at enhancing the functionality of traditional doorbells. With the integration of an LCD counter and click history feature, this doorbell not only serves as a communication tool but also provides valuable insights into its usage. The doorbell tracks the number of times it is pressed throughout the day, logs the date and time of each click, and displays this information on an LCD screen. This helps users keep track of visits, improves home security by offering a record of interactions, and adds a modern technological touch to home entry systems.

Let’s move on to how it’s working. The Smart Doorbell system is designed to detect, record, display, and store information every time someone presses the doorbell.

Main components involved:


●Microcontroller (like Arduino): Acts as the brain that processes everything. Without this, The whole system won't work. No brain = no counting, no display, no time record. Completely dead.

●Button: This is the doorbell that people press.

●LCD Screen: Shows the number of times the doorbell was pressed and the history. Without this, The doorbell can still count and store presses internally, but the user won’t see anything. No display, no real-time information.

●RTC (Real-Time Clock) Module: Provides the exact date and time when the button is pressed. Without this material, The system can still count how many times the button is pressed but it won't know the exact date and time of each press. Only the number will be recorded.

●Power Supply: Powers all the components.

●Wires, Connectors, and Casing: Connects and protects everything.

Step-by-Step Operation:

Button Press Detection

○ Someone presses the doorbell button.

○ The button sends an electronic signal to the microcontroller.

Microcontroller Processing

○ The microcontroller immediately detects this signal.

○ It increases the counter by one (example: from 5 to 6 presses).

Timestamp Recording

○ At the same time, the microcontroller asks the RTC Module for the exact date and time.

○ It logs the press event along with the timestamp into its memory (can be EEPROM, SD card, or internal memory).

LCD Display Update

○ The LCD screen refreshes to show:

■ Total number of times the doorbell has been pressed.

■ The latest history (such as "6th Press: 2025-04-27 03:15PM").

History Storage

○ Each button press and its timestamp are saved.

○ This allows the user to scroll through or view previous button presses using the LCD screen interface.

User Interface

○ The interface is kept simple and user-friendly.

○ It may display the latest presses one at a time or show a small list (depending on the screen size and design).

○ A reset button might also be available to clear the history and start fresh.
