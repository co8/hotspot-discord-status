# hds

## **Hotspot Discord Status** for the Helium Network Hotspots

## Getting Started

These instructions will give you a copy of the project up and running on
your local machine for development and testing purposes. See deployment
for notes on deploying the project on a live system.

### Prerequisites

Requirements for the software and other tools to build, test and push

- [Python v3.9+ Installed](https://www.example.com)
- [How to Use Crontab](https://www.geeksforgeeks.org/crontab-in-linux-with-examples/)
- [Discord Webhook for Python](https://pypi.org/project/discordwebhook/)

### Installing

A step by step series of examples that tell you how to get a development
environment running

Clone from Github

- clone link
- cd
- ...

Crontab

- Run every minute and at Reboot
- Change directory path to match your own
- Delete log file every Sunday at 0:00

  $ crontab -e
```
  \*/1 \* \* \* \* cd ~/hds; python3 hds.py >> ~/cron.log 2>&1

  @reboot ~/hds; python3 hds.py >> ~/cron.log 2>&1

  0 0 * * 0 rm ~/cron.log
```
Run directly from the directory

    cd ~/hds/
    python3 hds.py

End with an example of getting some data out of the system or using it
for a little demo

## Deployment

### Command line Arguments

```py
python3 hds.py report
```

- send a bobcat miner report, if bobcat_local_endpoint is set
  
```py
python3 hds.py reset
```

- resets by setting last sent and activity history


### Support this Project

If you find this project useful please consider supporting it

HNT: [14hriz8pmxm51FGmk1nuijHz6ng9z9McfJZgsg4yxzF2H7No3mH](https://explorer.helium.com/accounts/14hriz8pmxm51FGmk1nuijHz6ng9z9McfJZgsg4yxzF2H7No3mH)

### Seeking Grants and Bounties to Support this Project

I'm seeking grants and bounties to continue and extend development of this project.

### Optional Hardware
For convenience, I run this script on a Raspberry Pi Zero W

[**Raspberry Pi Zero W** Vilros Basic Starter Kit (Amazon)](https://amzn.to/3jWaUpF)