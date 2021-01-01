+++
title = "Docker download failure on Synology"
description = "Docker image download failure"
author = "Bart Vandyck"
date = "2020-12-31"
tags = ["synology"]
[[images]]
  src = "img/blog/synology_logo.jpg"
  alt = "Synology Logo"
  stretch = "stretchH"
+++


#  Docker image download failed on Synology
Date created: the 2020-12-26


When installing Home Assitant on my Synology 918, I was presented with the following notifition

<!--more-->

![[Pasted image 20201226235717.png]]

Checking the Docker Log for more information did not shet any light on the issue.  The only logged items  where of the type 'Information'

![[Pasted image 20201227000143.png]]

Checking internet access everything seemed fine, downloads via the Download station worked fine.  I do have my Synology configured to use Express VPN.  

Turning this off an re-trying the docker image seemed to solve the issue! 

Download success
![[Pasted image 20201226235740.png]]


This was tested on DSM version 6.2.3-25426 Update 3