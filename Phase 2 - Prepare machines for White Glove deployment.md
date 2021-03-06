# Phase 2 - Prepare machines for White Glove deployment and reseal machines for distribution

For each computer that we have prepared in [Phase 1](Phase%201%20-%20Harvest%20Hardware%20IDs%20for%20Windows%20Autopilot.md), please perform the following steps:

1. Boot up the computer.
    - Make sure the computer is plugged in.
    - Make sure it is connected to the Internet.
2. Reset this computer to OOBE condition:

    1. Open Start menu -> **Settings**.<br><br>![Settings](Assets/start-menu-settings.png)

    2. Click on **Update & Security**.<br><br>![Update & Security](Assets/update-and-security.png)

    3. Click on **Recovery**.  Under "Reset this PC," click the **Get started** button.<br><br>![Reset this PC](Assets/reset-this-pc.png)

    4. Click the **Remove everything** option.<br><br>
    ![Remove everything](Assets/remove-everything.png)

    5. Click the **Next** button.<br><br>![Warning!](Assets/warning.png)

    6. Click the **Reset** button.  (Note: This process will take some time to complete.)<br><br>![Ready to reset this PC](Assets/ready-to-reset-this-pc.png)
    
3. After the computer has rebooted itself, you will see the "Let's start with region" screen.<br><br>![Let's start with region](Assets/lets-start-with-region.png)
    - Do NOT press the "Yes" button.
    - Instead, press the **Windows key** five (5) times in quick succession.
4. On the "What would you like to do?" screen, select the **Windows Autopilot provisioning** option and press the **Continue** button.<br><br>![What would you like to do](Assets/what-would-you-like-to-do.png)
5. On the "Windows Autopilot Configuration" screen, press the **Provision** button.  (The provisioning process will take some time to complete.)<br><br>![Provision button](Assets/windows-autopilot-configuration-provision-button.png)
6. If the provisioning process is successful, you will see a *green* "Windows Autopilot Configuration" screen.  Press the **Reseal** button to reseal the machine.<br><br>![Reseal button](Assets/windows-autopilot-configuration-green-screen.png)
7. Once the machine is properly resealed, it will shut down itself.  We are ready to distribute this machine to the user at this point.
8. Repeat these steps for the next computer.

## Note
If the provisioning process failed in Step 6, you will see a *red* "Windows Autopilot Configuration" page.  Press the **Retry** button.  (Contact me if this occurs.)