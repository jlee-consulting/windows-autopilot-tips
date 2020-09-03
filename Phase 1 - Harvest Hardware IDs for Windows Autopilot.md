# Phase 1 - Harvest Hardware IDs for Windows Autopilot

For each new computer, please perform the following steps:

1. Boot up the new computer.  (Make sure the computer is plugged in.)

2. When prompted for the username, give it a name such as `tempadminuser` and a password.  (Once we are done with harvesting the hardware ID of this machine, we will do an OOBE reset in the next phase.)
3. Be sure to connect the machine to the Internet.
4. Make note of the *Service Tag Number* of this machine. Henceforth, we will refer to this as the `{service-tag-number}` and we will use it later to name our output file.
5. Harvesting the Hardware ID
    1. Launch PowerShell with elevated administrator privileges.
    2. Execute the following PowerShell commands:
        - Answer "Yes" if you get prompted.
        - Replace `{service-tag-number}` accordingly.
        <br><br>
        ```powershell
        Set-ExecutionPolicy Unrestricted

        md C:\hardwareid

        cd C:\hardwareid

        Install-Script -Name Get-WindowsAutoPilotInfo

        Get-WindowsAutoPilotInfo.ps1 -OutputFile {service-tag-number}.csv
        ```

6. Copy the resulting **C:\hardwareid\\`{service-tag-number}`.csv** file to my OneDrive shared folder.
7. You can now shut down this computer.
8. Repeat these steps for the next computer.

## Note
Once we have attained the **`{service-tag-number}`.csv** for all computers, I will take care of the device enrollment and user assignment from my end.

I will inform you when we are ready to begin the [next phase](Phase%202%20-%20Prepare%20machines%20for%20White%20Glove%20deployment.md).