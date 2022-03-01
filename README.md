# russia-must-be-stopped 

Easily support 🇺🇦 🇺🇦 Ukraine 🇺🇦 🇺🇦 by joining in the DDOS effort. Here's how, in **4** steps:



## 1. Set up a VPN.

Protect yourself by make your connections come from a different location than your own. I use Express VPN, but there are many alternatives. Here's what that looks like when it's up and running. I've got mine set to have all my Internet come and go through Phoenix, USA:

<img width="191" alt="Screen Shot 2022-03-01 at 7 42 41 AM" src="https://user-images.githubusercontent.com/16888908/156189619-60f2b140-344c-4f33-a14a-05cf8f9d6131.png">



## 2. Disable CORS in your browser.

This is essential: it allows the code to make the network connections. I use a separate profile in Chrome with the [Allow CORS](https://chrome.google.com/webstore/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf) extension. If you use Allow CORS (it's the easiest way I've found), just change Option 4 to `*`:

<img width="825" alt="Screen Shot 2022-03-01 at 7 40 35 AM" src="https://user-images.githubusercontent.com/16888908/156189279-78f2da97-dd69-404c-92b6-84488c047d44.png">

Then, be sure to actually turn on the extension itself. The "C" logo will appear orange:

<img width="145" alt="Screen Shot 2022-03-01 at 7 41 42 AM" src="https://user-images.githubusercontent.com/16888908/156189455-48270f70-4897-4bb2-b892-8b08d06d14ed.png">



## 3. Browse to [russia-must-be-stopped.html](https://codergator.github.io/russia-must-be-stopped/russia-must-be-stopped.html).

Here's [the source code](https://github.com/codergator/russia-must-be-stopped/blob/master/russia-must-be-stopped.html), if you want to examine it. It's pretty simple, IMO.


## 4. Enable mixed content.

At this point, the script is running, but can only connect to the sites that use `https`.
But some of these Russian sites are still on `http`. In order to hit those as well, we need
to enable "mixed content" (a mix of `https` and `http`). 

### Instructions for the Chrome Browser

First, click the lock to the left of the URL, then click **Site settings**:


<img width="1194" alt="Screen Shot 2022-03-01 at 7 54 30 AM" src="https://user-images.githubusercontent.com/16888908/156196409-fa9c5104-881b-4983-9588-4f907390c2c8.png">


Then, on the Site settings page, scroll down to the **Insecure content** setting:

<img width="654" alt="Screen Shot 2022-03-01 at 7 54 48 AM" src="https://user-images.githubusercontent.com/16888908/156196848-0a632eda-a024-49b0-b612-9aba541057ab.png">

Change it to **Allow**:

<img width="652" alt="Screen Shot 2022-03-01 at 7 54 58 AM" src="https://user-images.githubusercontent.com/16888908/156196908-fc585d69-ac85-4308-8823-18150622ea17.png">


Your browser will load all the URLs, even the ones over `http`.

