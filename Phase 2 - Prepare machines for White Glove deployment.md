# Phase 2 - Prepare machines for White Glove deployment and reseal machines for distribution

For each computer that we have prepared in Phase 1, please perform the following steps:

1. Boot up the computer.  (Make sure the computer is plugged in.)
2. Reset this computer to OOBE condition:
    1. Open Start menu -> **Settings**.
    2. Click on **Update & Security**.
    3. Click on **Recovery**.
    4. Under "Reset this PC," click the **Get started** button.
    5. Click the **Remove everything** option.
    6. Click the **Next** button.
    7. Click the **Reset** button.

    This process will take some time to complete.
    
3. After the computer has rebooted itself, you will see the "Let's start with region" screen.  Do NOT press the "Yes" button.  Instead, press the **Windows key** five (5) times in quick succession.
4. On the "What would you like to do?" screen, select the **Windows Autopilot provisioning** option and press the **Continue** button.
5. On the "Windows Autopilot Configuration" screen, press the **Provision** button.  (The provisioning process will take some time to complete.)
6. If the provisioning process is successful, you will see a *green* "Windows Autopilot Configuration" screen.  Press the **Reseal** button to reseal the machine.
7. Once the machine is properly resealed, it will shut down itself.  We are ready to distribute this machine to the user at this point.
8. Repeat these steps for the next computer.

## Note
If the provisioning process failed in Step 6, you will see a *red* "Windows Autopilot Configuration" page.  Press the **Retry** button.  (Contact me if this occurs.)