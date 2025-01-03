# armts
A Typescript to ARM compiler written in C++17

##  Running ARM programs
I rented an EC2 instance running Ubuntu 24.04 and used QEMU to emulate an ARM processor.
#### Preliminary setup
- `$ apt-get install gcc-arm-linux-gnueabihf`
- `$ apt-get install qemu-user`
#### How to run ARM programs
- `$ arm-linux-gnueabihf-gcc -static <your_file>.s -o <your_program>`
- `$ qemu-arm ./<your_program>`
