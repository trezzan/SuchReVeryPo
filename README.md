# . : SuchReVeryPo : .
**NO SPECIFIC README.MD WAS SPECIFIED FOR THIS WEEK, SO I AM GOING TO BUILD A SIMPLE RUBRIC.**

## MILESTONE 0
![](https://github.com/trezzan/SuchReVeryPo/blob/master/0.GIF)
*NOTE: I am unsure why the posted images are not animating. They were recorded via LICECap, and played when first recorded. I am not sure why they are static images now.*
Purpose: This step involved creating a GCloud account, and properly preparing our cloud based machines to process the honeypot data for us. Google includes a very effective set of instructions with cmd by cmd detail to get your cloud service running. Setting the regions and zones allow the machines to run in a relatively close server in order to give live feedback quickly. 
## MILESTONE 1
![](https://github.com/trezzan/SuchReVeryPo/blob/master/1.GIF)
Purpose: Having the GCloud platform setup is only useful if there is an admin console that can properly run it. In this we manually allow for our admin consoles to send and recieve data from our honeypots and remote connections. Firewall rules are setup to protect the admin console from attacks and port scans. If the console was not properly protected, then anyone with a thorough understanding of GCP could scan around for admin consoles and begin taking over many remote machines running around the world (in theory). 
## MILESTONE 2
Trouble: This is where my day took a very downward spiral. After establishing the SSH connection to my ubuntu machine, Https://github.com/RedolentSun/mhn.git was the next program to grab. Now, I downloaded the git just fine, but my machine refused to install the application. I started doing some digging, and the application had issue with some repositories that were created in order to run the application. Specifically, the MongoDB repo had a bad certification, and neither my VM nor my host wanted to work aroudn it. Runnung argments like --allow-unauthorized had no effect. Install failed. Apt-get updates (not matter the arguments added) would not run. The installer had added a like to my sources.list file, and that was crippling my ability to work around any application installation. I tried reinstalling my certificates to get a newer one, but that also had no effect. 

![](https://github.com/trezzan/SuchReVeryPo/blob/master/failure.GIF)

With this, I was stalled at this point in our excersize, and could not move forward. Between the Assignment section, and the Lab section, I had invested over 6 hours in one day (a nearly impossible feat as per my schedule, thank God for holidays), and was quickly realizing that I was running out of time to spend troubleshooting. I am **so very** disheartened to toss in the towel, but I decided that I cannot continue with this particular assignment. 

Instead, I will be writing the prupose for each following Milestone from this assignemnt in the hopes that I can get some credit from Facebook/Codepath from it. I feel like a fool (becuase I am one), and am very reluctant to do this. 

## MILESTONE 3

## MILESTONE 4

## MILESTONE 5

