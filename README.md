# Reset Logic Pro Trial - Educational Purpose Only

## Introduction

We found a problem with how Apple counts the remaining days of the Logic Pro X trial. We discovered a file that gets created when we download and start using the trial version from the App Store. This GitHub Repo has the script that can bypass this file-based security protocol. However, we don't support or encourage the use of such scripts as it can be illegal and pose security risks.

We do not support piracy and the use of cracked software. Piracy is a violation of intellectual property laws and can harm the creators and the industry as a whole. Moreover, cracked software may contain viruses, malware, or other harmful code that can compromise the security of your device or data. We strongly encourage our users to respect intellectual property rights and to only use licensed software and legal means of accessing digital content.

I must clarify that we do not condone the practice of extending the trial period of any software, including Apple Logic Pro X. We appreciate the affordability and feature-richness of Logic Pro X. We also believe it is important to respect the licensing terms of the software and support its developers by purchasing a legitimate license.

We ourselves are legitimate owners of Logic Pro X because we understand the value of investing in high-quality tools to support our creative endeavors.

However, it is important to note that extending the trial period of any software without a legitimate license is illegal and unethical. While it may seem like an easy solution, it poses risks to both the user and the developers.

## Where Logic Pro Stores the Trial Counter

Logic Pro X trial counter is stored in a hidden file named **lpxuserdata** under **Library > Application Support**
This file gets generated as you open logic pro for the first time and continues keeping the count until the trial expires.
Since this is a hidden file, a regular user may not be able to locate this easily.
Also it is a little tricky to navigate to the **Library** folder.

Therefore we encourage using the **Terminal** app on your mac.

## Terminal Commands to Reset Logic Pro Trial

Follow the steps below to open Terminal

1. Press ***Cmd+Space***
2. Type **Terminal**
3. Press Return or Enter

Write the following command on Terminal and hit Return

> sudo rm -r ~/Library/Application\ Support/.lpxuserdata

Write your password if it prompts for.

### Important

1. Make sure Logic Pro X is not running (in foreground or background) while performing this operation.
2. The "Trial" mark on the splash screen shall not vanish.
3. Every time you start Logic Pro, you shall still see the screen reminding you to buy and showing the count.
4. Remember to repeat the steps everytime before you hit the 90th day.
5. This process works for Final Cut Pro as well, just replace the .lpxuserdata with .ffuserdata
6. An advance user may create a Cron Job to automate this process of running the script every, let's say, 80th day

## Conclusion

If you love Logic, please support the developers by purchasing an original license. It is the cheapest Fully Functional Professional DAW available and let's celebrate that.
