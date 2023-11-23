# Q&A

This is the general Q&amp;A section for all the apps I wrote. Here are some most mentioned problems and answers that might help you.

## Are your apps supporting Intel?

- Sorry. All my apps are now M chip Macs only. I have tried to build X86 apps on my M1 Macbook Pro, but it seems to be impossible, or at least out of reach from my side. 

## Why is it saying the app is not compatible with the system?

- Maybe you are using an Intel Mac, and that's the reason. The architectures are totally different.

## Why is it keep saying that the app is broken and suggest to throw into waste basket?

- The core reason here is the same for all indie apps distributed on GitHub. There are many developers like me, didn't buy the certificate from Apple, so when the system is checking the app, it alerts.

- **Solution**: The solution is easy. 

1. First, open the ```System Settings``` and go to ```Privacy & Security```. Under security part, you might see ```Allow applications downloaded from```, then you should choose at least ```App Store and identified developers```. There is a hidden option which is called ```Anywhere```, and it can be shown by using command in Terminal. You may enter the following command in Terminal: ```sudo spctl --master-disable```. Input your password, then you should see the option in the panel. You may choose ```Anywhere``` option as well.

2. Second, when opening a new app with alert showing up, there should be an option down in the ```Security``` panel to let you allow or deny. Choose ```Allow```then.

3. Third, if it still doesn't work, open Terminal and enter the command ```sudo xattr -r -d com.apple.quarantine ``` (don't miss the space at the end), then open the Application folder in Finder, drag and drop the app you would like to open into the Terminal window. This is to get the Finder path of target app. Now it should look like ```sudo xattr -r -d com.apple.quarantine /Applications/Broccoli.app```, taking Broccoli the app as an example. Enter it, then Terminal would require your password. And everything would be fine.

## Are these apps all FREE?

- Not all apps are free. Some might be paid only and some have Pro versions that are paid apps. But all apps are open-sourced.

## Are these apps all open-sourced?

- Yes. You can read the code on GitHub.

## I don't understand what is this app for.

- I hope I can explain to you pretty clearly but all apps are restricted to some certain need scenarios. I have written a lot of automation apps and they actually can be done in many ways, but I only found it easy and simple being in the app form. 

- E.g. Coconut syncs all photos from Finder path to Photos.app, and this is pretty important since my universal clipboard is not always working properly. But if you have a normal Handsoff function, this might not solve your problem. 

- E.g. Broccoli has a function to use third-party APIs and their endpoints, which is due to the fact that OpenAI's service is denied in many countries. If you are lucky enough to have the official service, then Broccoli might not be your first choice in this case. BTW Broccoli also has many other functions so you may see if there is anything you like.

## Will the permission degrade my privacy status?

- I will promise that all apps written by me and distributed directly from me are safe apps. Despite Orange the app may need Internet to fetch RSS and apps that embed AI function like Broccoli and Strwberry, others only need Internet for update checking. Especially for those automation apps, you can run them with no Internet. And there is no need to worry about sending your private data to the public.

## What if the guide above cannot solve my problem?

- You may contact me directly in many ways:
	- Email: sweeter.02.implant@icloud.com or ryanthehito@protonmail.com
	- X (Twitter): https://twitter.com/ryanswindows
	- Reddit: https://www.reddit.com/user/Plenty-Reference69

- You can choose one way to tell me about your problem and I will send you feedback ASAP. Thanks!!🙏