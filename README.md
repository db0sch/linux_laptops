# linux_laptops

A list of linux friendly laptops

![boromir_meme](https://i.imgflip.com/18xlvc.jpg)

## important rules
- avoid consumer laptops. they might carry some bios/uefi restrictions which prevent installing linux on these machines. professional series laptops are more suitable (but might be more expensive)
- avoid touch screen:
  1. linux UI not very touch compatible
  2. might create issues
- be careful with Nvidia graphics card: always prefer intel graphic cards as they provide open source drivers. Nvidia can cause issues which are difficult to debug. The situation might be better now though (with the `nouveau` drivers). I invite you to check the best linux compatible nvidia cards on the web (more info here: https://wiki.archlinux.org/index.php/NVIDIA)
- avoid exotic brands (unless they are officialy supporting linux). The common models and brands are well documented by the community. Easier for troubleshouting.
- USB-C is eating the world (of laptops). Some laptops have just one port. So keep that in mind if you need retro-compatibility with older hardware, and even to connect to a beamer (might need to purchase an adapter)
- Some manufacturer are now configuring the hard disks in Raid, which can make the linux installation more complex (especially for Dual Boot).

## brands

### DELL

The XPS series:
- XPS 13 | [Dell website](http://www.dell.com/en-us/work/shop/dell-laptops-and-notebooks/xps-13/spd/xps-13-9360-laptop)
  *  2x USB 3, 1x USB-C and 1x SD card slot
- XPS 13 Developper Edition | [Dell website](http://www.dell.com/en-us/shop/cty/pdp/spd/xps-13-linux)
  // The developper edition comes with Ubuntu linux pre-installed (no windows though)

The Latitude series:
- 5000 and 7000 models | [Dell website](http://www.dell.com/en-us/work/shop/dell-laptops-and-notebooks/sf/latitude-laptops)

### LENOVO

Avoid consumer laptops from Lenovo at all cost. For two reasons:
- They ship consumer laptops infected with adware / spyware
- They sometimes add some restrictions to avoid linux installation

Go with the thinkpad models: http://www3.lenovo.com/us/en/think/
as they are known for the compatibility with linux (many sys admin use thinkpad on linux)

The X series:
- X270 (and older version, until x220)
- X1 Carbon (quite expensive though)

The T series:
- T470 (and older version, such as T450)
- T470s (slim version)

Yoga series:
- Yoga 720 13" (1 USB-C for power, 1 extra USB-C, 1 USB 3, no HDMI)
  * it's shipped with a RAID system, which might be an issue to install linux. If you disable it in the bios, it will mess with Windows (might need to completely ditch Windows)

### HP

According to HP, their laptops are compatible with Ubuntu -> [HP website](http://www8.hp.com/us/en/campaigns/ubuntu/index.html)

I have no experience with installing linux on a HP computer. But then again, try to avoid consumer, and look at the pro models.

### System76

System76 is a linux installed computer manufacturer. It means their products will never ship with Microsoft Windows.
So if you want to keep Windows on the side (dual boot) for gaming or running any non cross platform apps (Photoshop, Adobe Premiere, ... etc), you'll should have a look at other manufacturers.

[website](https://system76.com/laptops)

All their laptops are compatible with linux (at least ubuntu and derivatives), no wrong choices here.

### Asus

  - Asus zenbook 13"
    * only 1x USB-C port. Might need an adapter for other ports
  - Asus R415UQ
    * Nvidia graphics inside, but driver seems to work well
  - Asus R510J
    * Nvidia 800+ series graphics inside, but driver seems to work well

### Acer

No experience in installing linux on Asus laptops.
Please feel free to contribute to this repo if you have information on this.

### Apple

Since the MacTel (Mac + intel) revolution, it is now possible to install Linux on Apple laptops.
But it seems that Apple made it more difficult on their 2017 models.

But models previous to 2016 should be Linux compatible. (not as seamless as Dell or Thinkpads, but should work).

### Other linux compatible manufacturers

- Alpha - [website](https://alpha.store/product/litebook-laptop/)
- ZaReason - [website](https://zareason.com/Laptops/)

### Chromebooks

ChromeOS is a Gnu/Linux based OS.
It is then possible to install a "real" linux distribution on it.

GalliumOS: https://galliumos.org/
You can check the hardware compatibility with Chromebooks here: https://wiki.galliumos.org/Hardware_Compatibility

There is also [crouton](https://github.com/dnschneid/crouton), but it actually run a linux alongside ChromeOS. So you can switch between the two. Drawback: it consums lots a memory. (And you don't really need to OS at the same time)

## Distributions

### Ubuntu
At [le wagon](https://www.lewagon.com), we advise students to install [Ubuntu](https://www.ubuntu.com/) in dual boot along with their legacy OS (Microsoft Windows). We even have a full setup tutorial for this: [le wagon setup](https://github.com/lewagon/setup)

### ElementaryOS
Based on Ubuntu, and that's what I use daily on my Lenovo Thinkpad x250. Works out of the box, flawlessly.
As it's based on Ubuntu, all the tools we use at Le Wagon are compatible.
I chose this one for its interface simplicity, and it is lightweight (good for energy management on laptops).
By far, Pantheon is the most elegant and beautiful Desktop Environment i've tried (the second one is Gnome, but a bit more heavy I think).

### Linux Mint
Never tried it, but several students/alumni use it. Base on Ubuntu as well. Seems to work perfectly.

### Ubuntu derivatives (Lubuntu, Xubuntu, Ubuntu Mate)
I only tried Ubuntu Mate. Works perfectly. Ugly though ;-)

### OpenSuse
I tried it. Works well. Especially `Tumbleweed` (rolling release distro). Always update to date with cutting edge packages.
But not same package manager as Ubuntu, and not exactly the same architecture. Can be tricky to have Le Wagon steup working on it.

### Arch
Never tried it. I know at least one student who installed it. Very advanced. Do not try it unless you understand well Linux.

### Fedora / CentOS
Never tried. Might be good. But same issues as OpenSuse. Not same architecture. Might be tricky to get Le Wagon setup to work on it.

### Solus
New. Looks promising.
One alumni is using it, works well.
(just a incompatibility with Ruby 2.3.4 and the kernel, fixed in 2.4.1)

List of supported device for Solus: https://solus-project.com/articles/hardware/laptops/en/

## Resources

Some resources for compabitility, tips and tutorials for laptops:
- [linlap](http://www.linlap.com/)
- [linux on laptop](http://www.linux-on-laptops.com/)
- [archLinux / laptops](https://wiki.archlinux.org/index.php/Category:Laptops) | per brand and models information
- [archlinux / laptop main page](https://wiki.archlinux.org/index.php/laptop)

