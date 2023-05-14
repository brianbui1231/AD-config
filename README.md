#                                             Active Directory Configuration Home Lab

## Overview

<p> This is a simple manual or lab environment of how to integrate the usage of Virtual Machine in a supported operating system such as Windows. In this lab, we will be using multiple Windows 10 VMs with Windows virtual machine server from Microsoft Azure to depict the utilization of user authentication and authorization within an active directory (AD). The essential goal of this lab is to give knowledge on AD in an environment such as Windows using their personally built tools and other third-party software that you might use. This is significant because most of the enterprise or business models use Window domain AD to ensure their network and data are secured. </p>

##  Requirements

* A computer or laptop that supports multiple operating systems
* Virtual Machine such as <a href="https://www.virtualbox.org">Oracle Virtual Box</a>
* A disk image of <a href="https://www.microsoft.com/en-us/evalcenter/download-](https://www.microsoft.com/en-us/evalcenter/download-
windows-10-enterprise">Windows 10</a>
* Make sure to enable virtulization in your BIOS

## Hypervisor Configuration

<ol>
  <li>Open your prefered hypervisor, I'm currently using a free one, Virtual Box. </li>
  <img src="https://github.com/brianbui1231/AD-config/blob/main/AD%20pictures/AD-1.png" /img>
  <li>Download ISO image of <a href="https://www.microsoft.com/en-us/evalcenter/download-windows-10-enterprise">Windows 10</a> if you haven't done so <br/> $~~~$ Click the 64 bit with your prefered language</li>
  <li>Once you finished downloading the image, go to your hypervisor and there should be a button to add your downloaded ISO image. In this example, click "new" </li>
  <img src="https://github.com/brianbui1231/AD-config/blob/main/AD%20pictures/AD-2.png" /img>
  <li> After clicking "new", it will prompt you to enter a name of your choice. In this prompt, input the downloaded Windows 10 ISO image under "ISO image"</li>
  <img src="https://github.com/brianbui1231/AD-config/blob/main/AD%20pictures/AD-3.png" /img>
  <li> Then hit next and enter your desired username and password, leaving everything else default. Otherwise you can also leave the username and password default as well. Click next when finished</li>
  <li> By default, you can leave RAM and CPU processors as is, however, if your PC or laptop can handle more, I would highly recommend adding more to make installing and functionally faster specifically CPU processors. In this example, I am keeping RAM default and adding more processors to 4. </li>
  <img src="https://github.com/brianbui1231/AD-config/blob/main/AD%20pictures/AD-4.png" /img>
  <li> The next step is adding virtual disk storage for our VM so it can install all required programs to run Windows 10. The minimum disk storage is 16 GB to install Windows 10. In this example, I'm setting it to 25 GB. Adjust to your preference.
    <img src="https://github.com/brianbui1231/AD-config/blob/main/AD%20pictures/AD-5.png" /img>
  <li> click next and then finish if you feel like everything is good and fine. Then it should start up a virtual Windows 10 and doing the normal setup</li>
  <li> You should be prompted to enter your prefered language and country keyboard</li>
  <li> Click next and accept terms of service. Then make sure to choose "Custom: install Windows only"</li>
  <li> Then you will prompted for disk allocation, hit next. </li>
  <li> Windows 10 will now install and the speed of download will depend on your computer specs and how much you allocate CPU processors from your host OS.</li>
  <img src="https://github.com/brianbui1231/AD-config/blob/main/AD%20pictures/AD-6.png" </li>
  </ol>
  
## Post installation Notes
* If you encountered an error along the way, most likely you didn't allocate enough disk space which is 16 GBs.
* Another error you might get is if the VM on bootup says license cannot be detected. Try rerunning the whole setup from beginning and not selecting an inital ISO image, therefore leaving it blank. Then during Windows installation, it will ask you choose boot image, select the Windows 10 ISO image you installed earlier.

## Windows 10 server 2022 configuration

<p> There a couple options you can do for creating a server</p>
<ul>
  <li> Get the Windows 10 server ISO image from the Microsoft website</li>
  <li> OR use Azure's virtual machine host to create a Windows 10 server </li>
  </ul>

<p> I'm going to be using Azure's virtual machine to create my Windows 10 server </p>


  
