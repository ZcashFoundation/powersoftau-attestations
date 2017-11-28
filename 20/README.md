
Date: 2017-11-28
Name: Zaki Manian
Location: Palo Alto, CA, USA

I used Bunny and Xob's Novena Laptop as my compute node for the Powers of Tau ceremony. The Novena is fully open source laptop that avoid proprietary drivers and firmware where possible. This was an appealing platform because it adds a platform without Intel ME to the mix.

I used the stock debian image. I reinstalled image and removed the wifi and bluetooth hardware.

Rust and cargo were installed via rustup.

I attempted to reproducibly build compute via path remapping.

zaki@novena-global-present:~/powersoftau$ rustc --version
rustc 1.23.0-nightly (827cb0d61 2017-11-26)

sha256sum target/release/compute
254ea87964e19f6c8434e868d83f1426e6a8b3397094f7f5c96de644b48663dd  target/release/compute

I performed the ceremony with Novena in a steel case. The Novena is quad core 32 bit armv7 platform so the compute took almost 8 hours The challenge and response were moved to the Novena via two seperate hard drives.

After completing the compute, I powered down the Novena before attaching the second hard drive.

The BLAKE2b hash of `./response` is:
	311cacac 3e74009d 452b54c1 10980a17 
	9dfdaee1 24bc7a79 d2713a27 922f35db 
	c054d7bd ea4d12a6 359a39c8 5906e684 
	590660aa 5e21b07e df743f19 914df9e9 

Photos of the Novena internals and steel cabinet setup are included.

