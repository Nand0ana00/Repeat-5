# Repeat-5

To build a browser-based alarm clock that plays random voice reminders starting 1 hour before the set alarm time, repeating every 5 minutes, with Pause, Stop, and Reset controls.

#Team name : CodeCroks

#Team members:
  1.Aswathi K R
  2.Nandana Vinu
  
   A web-based alarm clock that not only tells time but also helps users wake up effectively by:

    Starting voice reminders 1 hour before the alarm time.

    Playing a random motivational or wake-up message every 5 minutes using browser speech synthesis.

    Allowing users to pause, stop, or reset the alarm for better control.

problem: to eradicate the laziness to wake up

solution: we are generating a voice at each 5 min instead of alarm ringtones.it will help you to be in a routine everyday.

Technologies/components used:
For software:
  1.HTML,CSS,Javascript
  2.websearch API

#Implementation 

The Smart Alarm Clock is implemented using HTML, CSS, and JavaScript, and it leverages the Web Speech API to generate voice prompts. The implementation is structured into three main layers:
1. User Interface (UI) – HTML + CSS

    HTML (index.html) provides:

        A digital clock that updates every second.

        A time input for setting the alarm.

        Control buttons for Set, Pause, Stop, and Reset.

        A status display to show alarm status or notifications.
       CSS (style.css) enhances the look and feel by:

        Styling the clock using a digital font (Orbitron).

        Adding animations and glowing effects.

        Styling the buttons and layout to make it responsive and attractive.

2. Alarm Logic – JavaScript (script.js)

JavaScript handles the core functionality:
a. Digital Clock Display

    Uses setInterval() to update the time every second.

    Displays it using toLocaleTimeString().
b. Alarm Setup

    User sets alarm via an HTML time input.

    The script calculates the alarm time and pre-alarm start time (1 hour before).

    If the current time is within the pre-alarm window, it immediately starts voice prompts.

    Otherwise, it uses setTimeout() to delay the start of voice prompts until 1 hour before.

c. Voice Prompt Handling

    Uses the Web Speech API (speechSynthesis) to speak random phrases.

    Every 5 minutes, a new random message is spoken using setInterval().

    d. Final Alarm

    When the current time reaches the actual alarm time, it plays a final strong wake-up message and stops further prompts.

e. Control Buttons

    Pause: Cancels current speech and pauses voice alerts.

    Stop: Stops voice alerts and resets timers.

    Reset: Clears the alarm time, stops voice alerts, and resets UI.

3. Voice Prompts (Randomized)

    A predefined array of voice phrases is used:

const prompts = [
  "Hey! It's time to wake up!",
  "Rise and shine!",
  "Get ready for the day!",
  ...
];

    Each time a prompt is triggered, one is randomly selected.
#Flow Diagram (Summary)

[Set Alarm] → [Check Current Time]
       ↓
[Wait until 1 hour before]
       ↓
[Start speaking every 5 min]
       ↓
[At Alarm Time → Final Wake-up Voice]

🧪 Testing:

    Test with an alarm time 2–3 minutes ahead.

    Ensure the voice prompt starts 1 hour prior (or immediately if in the 1-hour window).

    Test Pause, Stop, Reset to ensure expected behavior.

#Installation:

The Smart Alarm Clock is a web-based project, so it doesn't require any special installation or external dependencies.

 Requirements:

    A modern web browser (Google Chrome, Firefox, Edge, etc.)

    Internet connection (optional, only needed for loading Google Fonts)

    No backend or server required
#Run:

🔹 Run Locally (offline)

    Download or create the project folder containing:

        index.html

        style.css

        script.js

    Open the index.html file using any web browser:

        Right-click → Open with → Chrome/Firefox/etc.

        Or double-click the file

    You’ll see the digital clock, and you can set the alarm and test the voice alerts

#Project documentation
<img width="899" height="943" alt="image" src="https://github.com/user-attachments/assets/d43c26d8-dc91-4698-a4f3-273ec87ea338" />

This is a stylish digital alarm clock interface featuring a glowing neon green LED-style display. It shows the current time (5:35:47 am), allows users to set an alarm time (e.g., 05:12 am), and includes functional buttons such as Set, Pause, Stop, and Reset. The UI also displays a final alarm alert at the bottom, indicating that the alarm is currently ringing.

Team contribution

1.Nandana Vinu setting web api search for random messages
2.Aswathi K R frontend


