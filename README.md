# KAY/O: Keep An Eye Out
![KAYO Thumbnail](https://github.com/kallui/kayo/assets/90471072/fd19891a-29d7-41fe-9a49-326d99ec2b6a)

Leaving your stuff unattended at a cafe or library? KAY/O watches it for you using just your laptop camera and object recognition to alert you if anything goes missing.

## Features
- **Object Recognition:** KAY/O uses YOLOv8 for object recognition to track your belongings.
- **Crash Detection:** The system includes a crash detection server to avoid thieves closing the application, or shutting down the laptop.
- **Alerts via Twilio:** Set up Twilio environment variables to receive text alerts straight to your phone.

## Demo
https://www.youtube.com/watch?v=aLop-hipPUE

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/aLop-hipPUE/0.jpg)](https://www.youtube.com/watch?v=aLop-hipPUE)

## Setup
1. Clone the crash detection server repository:
    ```bash
    git clone https://github.com/ST2-EV/kayo-cds.git
    cd kayo-cds
    ```

2. Set Twilio environment variables:
    ```bash
    export TWILIO_ACCOUNT_SID=xxxxxxxxxxxx
    export TWILIO_AUTH_TOKEN=xxxxxxxxxxxxx
    ```

3. (Optional but recommended) Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
    ```

4. Install requirements:
    ```bash
    pip install -r requirements.txt
    ```

5. Run the application:
    ```bash
    python ui.py
    ```
