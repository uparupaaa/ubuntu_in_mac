# ubuntu_in_mac
How to i nstall Ubuntu on a Mac(T2 Linux version)

if you want to install Ubuntu on a Mac(2019) in dual-boot mode, follow the steps below.

1. Download the Ubuntu ISO file from https://jp.ubuntu.com/download
2. Flash the ISO file as an OS image to a USB memory stick using BalenaEtcher.
   (The OS image size is about 6GB, so use a USB drive of at least 8GB.)
3. Create a new partition for Ubuntu.
   1. open disk utility.
   2. select macos device.
   3. click "Partition" and open the pi chart view.
   4. click "+" and choose "Add Partition".
   5. if you can afford it, please allocate 40GB(it's plenty of memory).
   6. set the Format to ExFAT.
   7. wait a few minutes for the partitioning to complete.
4. Restart your Mac and hold the Option key until the EFI boot screen appears.
5. Select the non-macOS drive to boot from the USB installer.(Wi-Fi is not required.)
6. If you see a security lock message, lower the security level from Full or Medium to Reduced, then restart from step 4.
7. Proceed with the installation.(be careful when choosing the installation disk - if you select Erase Entire Disk, macOS will be deleted.)
8. After installation, open the Treminal.
9. To enable Japanes input, run the following command and then restart:
```
sudo apt update && sudo apt install ibus-mozc
```
10. If Wi-Fi, keyboard, or touchpad do not work, download t2_linux.sh and run:
```
bash path/to/t2_linux.sh
```
11. Restart
12. Installation complete!
