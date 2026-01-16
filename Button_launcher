from gpiozero import Button
from signal import pause
import subprocess

button = Button(17, pull_up=True)

def run_external_file():
    print("Starting another Python file...")
    subprocess.Popen(["python3", "/home/pi/program_to_run.py"])

button.when_pressed = run_external_file

print("Waiting for button press...")
pause()
