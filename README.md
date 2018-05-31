# . : SuchReVeryPo : .
**NO SPECIFIC README.MD WAS SPECIFIED FOR THIS WEEK, SO I AM GOING TO BUILD A SIMPLE RUBRIC.**

## MILESTONE 0

![](https://github.com/trezzan/SuchReVeryPo/blob/master/0.GIF)
*Note: I am unsure why the posted images are not animating. They were recorded via LICECap, and played when first recorded. I am not sure why they are static images now.*

Purpose: This step involved creating a GCloud account, and properly preparing our cloud based machines to process the honeypot data for us. Google includes a very effective set of instructions with cmd by cmd detail to get your cloud service running. Setting the regions and zones allow the machines to run in a relatively close server in order to give live feedback quickly. 

## MILESTONE 1

![](https://github.com/trezzan/SuchReVeryPo/blob/master/1.GIF)

Purpose: Having the GCloud platform setup is only useful if there is an admin console that can properly run it. In this we manually allow for our admin consoles to send and recieve data from our honeypots and remote connections. Firewall rules are setup to protect the admin console from attacks and port scans. If the console was not properly protected, then anyone with a thorough understanding of GCP could scan around for admin consoles and begin taking over many remote machines running around the world (in theory). 

## MILESTONE 2

Trouble: This is where my day took a very downward spiral. After establishing the SSH connection to my ubuntu machine, Https://github.com/RedolentSun/mhn.git was the next program to grab. Now, I downloaded the git just fine, but my machine refused to install the application. I started doing some digging, and the application had issue with some repositories that were created in order to run the application. Specifically, the MongoDB repo had a bad certification, and neither my VM nor my host wanted to work aroudn it. Runnung argments like --allow-unauthorized had no effect. Install failed. Apt-get updates (not matter the arguments added) would not run. The installer had added a like to my sources.list file, and that was crippling my ability to work around any application installation. I tried reinstalling my certificates to get a newer one, but that also had no effect. 

![](https://github.com/trezzan/SuchReVeryPo/blob/master/failure.gif)
*Image Note: This is an animated clip RECREATING the processes that I went through attempting to update certs, work around installers, and try every argument to bypass bad certificate errors. I have learned a LOT about the apt-get function in linux.*

With this, I was stalled at this point in our excersize, and could not move forward. Between the Assignment section, and the Lab section, I had invested over 6 hours in one day (a nearly impossible feat as per my schedule, thank God for holidays), and was quickly realizing that I was running out of time to spend troubleshooting. I am **so very** disheartened to toss in the towel, but I decided that I cannot continue with this particular assignment. 

Instead, I will be writing the prupose for each following Milestone from this assignemnt in the hopes that I can get some credit from Facebook/Codepath from it. I feel like a fool (becuase I am one), and am very reluctant to do this. 

## MILESTONE 3
 
Purpose: Now, we need to create our first honeypot. We have the ability to run virtually unlimited (that could be pricey) with different purposes and settings. The important thing to remember is that they are all being virtualized, so we can use tiny specifcations to minimize our machine footprint and run more with out Google subscription. 

*Sidenote: I wonder if running honeypots in an environment like Docker could work. That would require virtually 1% overhead and could prove to be very useful*

Milestone 3 is nearly identical to Milestone 1 where we are using (so kindly provided) settings to get an Ubuntu machine virtualized in our cloud environment. This seems fairly cut and dry. Upon inspecting the instructional arguments, it seems that the install settings are the same as the mhn admin console machine. The main difference is in the naming, obviously substituting 'mhn-admin' for 'mhn-honeypot-1. The f1-micro argument is specific to GCF and specifies Google's more tiny machines that do not have much power. 

Doing some research, MHN stands for modern honey net. It is an open sourced option for creating honeypots just like ours. MHN supports the following open source honeypots and network sensors: Dionaea, Conpot, Cowrie, Amun, Glastopf, Wordpot, ShockPot, Elastichoney, p0f, Snort, Suricata. Other honeypots or sensors, even home-grown ones, can easily be added as well. MHN offers a ready to use REST API and supports the hpfeeds protocol making it straightforward to integrate with other solutions. Integration with other Anomali products is a breeze and this brings additional standards like CEF and STIX support to the table.
 
## MILESTONE 4
 
Purpose: At this point, we have an admin machine and a honeypot machine, but no running services or applications. Now, we need to install the honeypot framework to our honeypot machine. MHN has done fairly well to intgrate their installation and initialization into the GCF. There are a series of instructions to install the MGN specification (we are using Dinoaea in this scenario). We use the wget command to download the honeypot framework, we learned about wget in the labs which is cool. Once that is said and done, the honeypot can communicate with our mhn admin console and give updates on its progress and status. 
 
## MILESTONE 5
 
Purpose: Now we can do a simple port scan from outside our honeypot (assuming you remember the IP). You'll find some really fun ports open, and this is intentional. Checking the admin console shows that attacks from yourself and accross the internet. Now, if they are just port scans, then it may just be harmless. However, it is possible that third party bad actors could be trying to map an attack vector. Especially if you see more advanced attacks like ICMP requests of various flavors and requests for SSH, telnet, VNC, etc. 

These milestone sysnopsyes were the best I could do to follow along and learn about the honeypot process without dumping another 6 hours into trying to get the console installed. Hopefully, I can get some redemption of credit for this. 
 
