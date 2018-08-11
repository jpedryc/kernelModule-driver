# kernelModule-driver
Example kernel module (linux driver) based on https://www.apriorit.com/dev-blog/195-simple-driver-for-linux-os
and http://freesoftwaremagazine.com/articles/drivers_linux/

# Kernel used 4.15.0-29-generic

# Build

`make`

# Check module info
`sudo modinfo hello.ko`

# Load kernel module
`sudo insmod hello.ko`

# Check module
`sudo lsmod | grep hello

# Check logs
`sudo journalctl --since "1 hour ago" | grep kernel

# Disable module
`sudo rmmod hello`