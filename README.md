# PolarisBiosEditor v1.6.8

### Important: You need to disable SecureBoot / Activate CSM in your
### Motherboard UEFI because the modification will make
### the cryptographic signature invalid.

If you don't trust the EXE just build on Linux with ```sh build.sh```. Quick and easy.

For donations or other requests please contact me by email: shomi199870@gmail.com



0/58. If your AV warns you about a virus/trojan, consider it as false positive.

Fork from lojkinKot

works on linux with mono, executable is build against .net 3.5

one click timing feature should be used with care, it maybe not stable for you

please build the executable yourself or decompile the existing one if you don't trust

### v1.6.8
- Fixed Samsung Uber-Mix strap
- support for ("MT51J256M3", "MICRON");
              ("EDW4032BAB", "ELPIDA");
              ("H5GC4H24AJ", "HYNIX_1");
              ("H5GQ4H24AJ", "HYNIX_2");
              ("H5GQ8H24MJ", "HYNIX_2");
              ("H5GC8H24MJ", "HYNIX_3");
              ("K4G80325FB", "SAMSUNG");
              ("K4G41325FE", "SAMSUNG");
              ("K4G41325FC", "SAMSUNG");
              ("K4G41325FS", "SAMSUNG");
### v1.6.7
- created solution and project files for ide
- support for device id 0x67ef
- better timings for micron memory
- firmware signature test / firmware signature in ascii
- editing of bios message (experimental)
- online check for new versions
- online display of developer notice

### v1.6.6
- support for rx550 device id 0x699F

### v1.6.5
- support up to 48 entrys in the timings table (more than 2 memory vendors)

### v1.6.4
- elpida timings fixed
- K4G41325FS memory support

### v1.6.3
- timing modification starts now at 1500 instead of 1750
- device id 67FF now also supported

### v1.6.2
- experimental: ubermix timings are now also applied to 4g SAMSUNG vram (K4G41325FC, K4G41325FE)
- timing modification starts now at 1750 instead of 2000

### v1.6.1
- hynix memory H5GC8H24MJ now recognized (same timings as H5GQ8H24MJ)

### v1.6
- window resizes properly now
- memory vendor detection
- one click timing patch (samsung, hynix, elpida, micron)

### v1.5
- added FanControlMode setting
- implemented some timing editor related code (not usable yet)

### v1.4.1
- replaced WPF components with Windows Forms to archive mono compatibility

Contribution from Sebohe:

### Build Dependencies

Ubuntu 16.04.2:

```
sudo apt-get install mono-complete
```

Arch Linux:

```
yaourt -Sy mono48
```
### Building

```
sh build.sh
```

### Executing

Just change your working directory to the PolarisBiosEditor and execute:

```
./run.sh
```
