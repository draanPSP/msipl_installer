# MS IPL Installer

A Python script to install IPL code on PSP MemoryStick

# Usage
It is required to run the script as an Administrator on Windows or as root on UNIX-like systems due to required low-level access to the drive.
On Windows, you have to provide the physical drive number via `--pdisk` argument.
On UNIX-like system, you have to provide the drive's device name via `--devname` argument.

# Examples

## Print info about the drive
```bash
python3 msipl_installer.py --devname sdc --info
```

## Clear the IPL space on the drive
```bash
python3 msipl_installer.py --devname sdc --clear
```

## Extract the IPL currently installed on the drive
```bash
python3 msipl_installer.py --devname sdc --extract out_ipl.bin
```

## Insert the provided IPL on the drive
```bash
python3 msipl_installer.py --devname sdc --insert in_ipl.bin
```
