# DDoS'ing for beginners: DDoS Russia in 4 easy steps 

Support 🇺🇦 🇺🇦 Ukraine 🇺🇦 🇺🇦 by joining in the DDoS effort! Here's how, in **4** steps.

**System Requirements**

I'm running this on a 2011 Mac Mini with 4GB RAM. 
You can tell you're running out of memory if the console shows "insufficient resources" errors.
Open up an issue if that's the case. We could make the memory usage configurable.



## 1. Set up a VPN.

Protect yourself by make your connections come from a different location than your own. I use Express VPN, but there are many alternatives. Here's what that looks like when it's up and running. I've got mine set to have all my Internet come and go through Phoenix, USA:

<img width="191" alt="Screen Shot 2022-03-01 at 7 42 41 AM" src="https://user-images.githubusercontent.com/16888908/156189619-60f2b140-344c-4f33-a14a-05cf8f9d6131.png">



## 2. Disable CORS in a new Chrome browser profile.

> These instructions use Chrome because it's secure and not hard to configure.

This is essential: it allows the code to make the network connections. Follow these instructions to create a **new, a separate profile** in Chrome for this.

⚠️ **Do not simply disable CORS in your current browser profile.** ⚠️

Continue following the instructions to keep yourself safe. To create the new profile, first click your current profile avatar in the upper right corner. Then click **+ Add** to add a new profile:

<img width="343" alt="Screen Shot 2022-03-01 at 11 13 23 AM" src="https://user-images.githubusercontent.com/16888908/156227020-12ab6639-c526-4858-a0c9-a32d7f2b39dc.png">

In the next screen, click **Continue without an account**:

<img width="732" alt="Screen Shot 2022-03-01 at 11 08 27 AM" src="https://user-images.githubusercontent.com/16888908/156225725-4bc3afe5-1c6a-4b83-bdad-aa6f3afb3a8f.png">

Now you can give the new profile a name:

<img width="732" alt="Screen Shot 2022-03-01 at 11 08 47 AM" src="https://user-images.githubusercontent.com/16888908/156225866-94fc3be6-9d17-4d49-a422-46c5c4946496.png">

Finally, you'll a new profile just for doing the DDoS'ing:

<img width="775" alt="Screen Shot 2022-03-01 at 11 12 10 AM" src="https://user-images.githubusercontent.com/16888908/156225941-5ba742b8-703c-45ed-919d-772349eb0532.png">

Now install [Allow CORS](https://chrome.google.com/webstore/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf) into your new profile. If you use Allow CORS (it's the easiest way I've found), just change Option 4 to `*`:

<img width="825" alt="Screen Shot 2022-03-01 at 7 40 35 AM" src="https://user-images.githubusercontent.com/16888908/156189279-78f2da97-dd69-404c-92b6-84488c047d44.png">

Then, be sure to actually turn on the extension itself. The "C" logo will appear orange:

<img width="145" alt="Screen Shot 2022-03-01 at 7 41 42 AM" src="https://user-images.githubusercontent.com/16888908/156189455-48270f70-4897-4bb2-b892-8b08d06d14ed.png">



## 3. Browse to [russia-must-be-stopped.html](https://codergator.github.io/russia-must-be-stopped/russia-must-be-stopped.html).

Here's [the source code](https://github.com/codergator/russia-must-be-stopped/blob/master/russia-must-be-stopped.html), if you want to examine it. It's pretty simple, IMO.



## 4. Enable mixed content.

At this point, the script is running, but can only connect to the sites that use `https`.
But some of these Russian sites are still on `http`. In order to hit those as well, we need
to enable "mixed content" (a mix of `https` and `http`). 

First, click the lock to the left of the URL, then click **Site settings**:


<img width="1194" alt="Screen Shot 2022-03-01 at 7 54 30 AM" src="https://user-images.githubusercontent.com/16888908/156196409-fa9c5104-881b-4983-9588-4f907390c2c8.png">


Then, on the Site settings page, scroll down to the **Insecure content** setting:

<img width="654" alt="Screen Shot 2022-03-01 at 7 54 48 AM" src="https://user-images.githubusercontent.com/16888908/156196848-0a632eda-a024-49b0-b612-9aba541057ab.png">

Change it to **Allow**:

<img width="652" alt="Screen Shot 2022-03-01 at 7 54 58 AM" src="https://user-images.githubusercontent.com/16888908/156196908-fc585d69-ac85-4308-8823-18150622ea17.png">

You'll probably have to reload the page to pick up the new setting. Chrome gives a helpful button for that:


<img width="517" alt="Screen Shot 2022-03-01 at 7 59 26 AM" src="https://user-images.githubusercontent.com/16888908/156197819-01d71815-fda8-4bed-a50d-4e00a9bdfa87.png">


And you're **done**. Your browser will load all the URLs, even the ones over `http`.



## 5. Verify it's working.

Welcome to step #5 out of 4. You should probably make sure this is actually working correctly. It took me several tries to get it right. To do this, open up the Javascript Console. On the Mac, it's alt-cmd-j. You can also right-click on the page, choose **Inspect**, and then switch to the **Console**. It should look like this:

<img width="1101" alt="Screen Shot 2022-03-01 at 7 59 56 AM" src="https://user-images.githubusercontent.com/16888908/156197919-77eb63aa-13ce-4683-91a2-9c02c304310e.png">

Uncheck **Group similar messages in console**. Now it should look like this:

<img width="1101" alt="Screen Shot 2022-03-01 at 7 59 52 AM" src="https://user-images.githubusercontent.com/16888908/156198025-762c200a-ddd2-4660-9882-6dabf4e351eb.png">

Notice how the browser is complaining about the mixed content, but it's going ahead and loading it anyway. Because I enabled it in Step 4.

But if your console looks like this, then you didn't properly enable mixed content. Go back and try again:

<img width="1097" alt="Screen Shot 2022-03-01 at 8 33 49 AM" src="https://user-images.githubusercontent.com/16888908/156198610-041df882-662a-416d-8490-0e323d44c7f1.png">

Any questions? Ask them in the [discussion forum](https://github.com/codergator/russia-must-be-stopped/discussions).


# Other similar projects and forks

* https://github.com/erkexzcx/stoppropaganda
* https://github.com/ajax-lives/NoRussian
