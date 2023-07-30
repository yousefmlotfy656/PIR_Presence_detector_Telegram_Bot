Arduino Presence Detector with Telegram Feedback
This arduino project demonstrates how to create a motion detection system using the ESP8266 NodeMCU that sends notifications to your Telegram account whenever motion is detected. By following this project, you can receive real-time alerts on your smartphone or computer from anywhere, as long as you have internet access. The ESP8266 board will be programmed using the Arduino IDE.

Project Overview
The project's main objective is to set up a motion detection system that integrates the ESP8266 NodeMCU, a PIR (Passive Infrared) motion sensor, and Telegram messaging service. Here's an overview of how the system works:

Create a Telegram bot for the ESP8266 NodeMCU to interact with.
Connect the PIR motion sensor to the ESP8266 NodeMCU.
When the motion sensor detects movement, the ESP8266 NodeMCU sends a warning message to your Telegram account.
You receive a notification in your Telegram account whenever motion is detected.
This project showcases how Telegram can be integrated into Internet of Things (IoT) and Home Automation projects to provide instant notifications and remote control capabilities.

Introducing Telegram
Telegram Messenger is a cloud-based instant messaging and voice over IP service that supports smartphones (Android and iPhone) and computers (PC, Mac, and Linux). It offers a secure and ad-free communication platform and allows users to create and interact with bots.

For this project, we'll create a Telegram bot that will enable the ESP8266 NodeMCU to send messages to your Telegram account.

Creating a Telegram Bot
Follow these steps to create a Telegram bot and obtain the bot token:

Download and install the Telegram app on your smartphone.

In the Telegram app, search for "botfather" and click on "BotFather" to start creating a new bot.

Type /newbot and follow the instructions to create your bot. Give it a name and username.

Once your bot is created, you'll receive a message with a link to access the bot and the bot token. Save the bot token, as it will be required for the ESP8266 to interact with the bot.

Get Your Telegram User ID
To ensure that only authorized users can interact with your Telegram bot, you can obtain your Telegram User ID. Here's how:

Search for "IDBot" in the Telegram app or open this link: t.me/myidbot.

Start a conversation with the bot and type /getid. You'll receive a reply with your user ID. Save the user ID, as you'll need it later in the tutorial.

Preparing Arduino IDE
Before programming the ESP8266 board, ensure that you have the Arduino IDE installed.

Follow these steps to install the necessary libraries:

Download the latest version of the Universal Telegram Bot Library by Brian Lough, which provides an easy interface for the Telegram Bot API.

Install the ArduinoJson library version 6.5.12.

Schematic Diagram
Wire the PIR motion sensor to your ESP8266 board according to the following schematic diagram:

Schematic Diagram

In this example, the PIR motion sensor's data pin is connected to GPIO 14 of the ESP8266.

ESP8266 Sketch
The provided Arduino sketch utilizes your Telegram bot to send a warning message to your Telegram account whenever motion is detected. To make the sketch work, insert your network credentials (SSID and password), the Telegram Bot token, and your Telegram user ID.

Note: Ensure that you have installed the necessary libraries mentioned in the tutorial.

With this setup, you can now receive notifications on your smartphone or computer whenever the motion sensor detects movement. This project serves as a foundation for more sophisticated IoT and Home Automation projects that leverage Telegram's instant messaging capabilities for real-time updates and remote control functionality. Feel free to customize and expand on this project to suit your specific requirements and ideas.