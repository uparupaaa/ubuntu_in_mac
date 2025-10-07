# ubuntu_in_mac
description how to install Ubuntu in Mac(T2_linux ver)

do you want to install Ubuntu in Mac(2019) in dual boot, do below

1. download ubuntu's iso file in https://jp.ubuntu.com/download
2. flash iso file as OS image to USB memory(OS image volume is about 6GB, so larger than 8GB) by "balenaetcher"
3. partition disk memory(where is installed Ubuntu)
   1. open disk utility
   2. select macos device
   3. push "Partition" and click pi chart
   4. click "+" and select "Add Partition"
   5. if you can afford it, please allocate 40GB(it's plenty of memory)
   6. select "ExFAT" for Format
   7. wait while partitioning(few minutes)
5. restart pc and keep pushing "option" button until the EFI screen is displayed
6. select non-macos disk(wifi is not neccesary)
7. if security is locked, change security strongness from strong or medium to weak(and restart from 5)
8. setting and install(carefully when you select the disk where Ubuntu is installed, if you select all delete, macos is deleted)
9. open terminal
10. japanese setting
'''
sudo apt update && sudo apt install ibus-mozc (and restart)
'''
