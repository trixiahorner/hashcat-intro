# *Intro to hashcat* #
This is a general introduction to hashcat, the powerful password cracking tool. The demonstration begins with generating md5 hashes and using hashcat to crack the password. Not only is this a basic 101 walkthrough of the hashcat tool, but it also serves to demonstrate why md5 hashing is not recommended for cryptographic security. 

### Install ###
- Download [the latest release of hashcat](https://hashcat.net/hashcat/) and use 7z to unpack. 
- **Running *hashcat* in virtual machine vs host OS:** *hashcat* takes advantage of a systems's GPU for it's parallel processing abilities (also used in gaming and AI). The GPU can perform more efficiently than the general purpose CPU. To put simply, the faster the GPU, the faster and more efficient *hashcat* will run.  It is possible to use *hashcat* inside of a virtual machine; however, it will use the CPU instead, making the process slower.

### Usage ###
- Features
  * open source
  * supports multiple algorithms
  * crack multiple hashes in parallel
  * support for Windows, Linux, and Mac OS
<br />
<br />

- Generate hashes and save to a file *(echo -n option: leave off trailing newline) (tr -d “ -”option deletes whitespaces and dashes)* <br />
   <img src="https://i.imgur.com/oL0yXSw.png" height="80%" width="80%" alt="hash generate"/>
- Use command *hashcat --help* for options. *(-m 0 specifies md5 hash mode and -a 0 straight attack mode)* <br />
  <img src="https://i.imgur.com/glwQR4I.png" height="80%" width="80%" alt="hashcat help"/>
- Results <br />
  <img src="https://i.imgur.com/JOlvFHJ.png" height="80%" width="80%" alt="hashcat results"/>
- Output results to a file using *-show* option <br />
  <img src="https://i.imgur.com/zLZYhKJ.png" height="80%" width="80%" alt="hashcat results"/>
