# GhostDelivery

Python script to generate obfuscated .vbs script that delivers payload (payload dropper) with persistence and windows antivirus disabling functions.
Heavy:

Downloads payload to TEMP directory and executes payload to bypass windows smart screen. Disables Defender, UAC/user account control, Defender Notifications, injects/creates Command Prompt and Microsoft Edge shortcuts with payload path (%TEMP%/payload.exe) to execute payload when opened, adds a scheduled task called "WindowsDefender" for payload to be run at login and obfuscates the vbs delivery script. This tool also has a serveo function to deliver obfuscated vbs script.
# Medium:

The medium option only delivers/executes payload, creates a scheduled task named "WindowsDefender" to run payload at login for persistence, disables UAC and injects/creates Command Prompt and Microsoft Edge shortcuts with payload path.
# Light:

The light option only delivers/executes payload, creates a scheduled task named "WindowsDefender" to run payload at login for persistence and injects/creates Command Prompt and Microsoft Edge shortcuts with payload path.
Prerequisites/requirements:

*Python 2.7, Modules imported in script. (random, sys, string, os, time, base64)
