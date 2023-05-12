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
  </ol>
