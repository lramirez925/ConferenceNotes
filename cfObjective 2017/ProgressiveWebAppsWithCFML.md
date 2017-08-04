# Building Progressive web apps using cfml
## By Miles Rausch - twitter: awayken

1. Problems. 
    1. Unreliable Networks. 
    1. No Backgorund Proccessing. 
    1. No background communication. 
    1. No Instalation
1. PWA Offers. 
    1. Web technology for native application experience. 
    1. service workers. 
        1. back bone of PWA. 
            1. JS thread running in background. 
                1. Good for background processes. 
            1. Programmable network proxy. 
            1. Decouples DOM and UI thread from work. 
            1. Uses promises for easy async actions. 
            1. Listens to events. 
                1. Registration -> UI/ Browser registers to worker event. 
                1. Installation -> event on instal. 
                1. Activation -> New service worker comes alive and kills old one. 
                1. Fetching and messaging events. -> Browser can listen to these. 
                1. Termination. 
            1. Requirements. 
                1. HTTPS (or localhost)
                1. Browser Support (Look at isServiceWorkerReady)
                1. Chrome or Firefox Dev Tools fro debiugggin and testing. 
                1. Requires you to start with basic app and then it enhances your app. (Due to browser support)

    1. CachStorage Api. 
        1. Offline first 
        1. Create named caches for domain. 
        1. Can add, delete, list keys and match 
        1. Fetch Api for network. 
        1. Built on promises. 
        1. Various strategies. 
            1. Cache only
                1. Always comes from cache. (font files, logos, non edited files)
            1. 
                Network only
                1. Form posts and not way to make it offline. 
            1. Cache to network fallback
            1. Network first then grab from cache. 
            1. Get from cache then update via network for future. 
            1. Offline Cookbook
    
    1. Fetch Api. 
    1. Install to Device. 
        1. Add to homescreen
            1. Requires manifest file. 
        1. Install banners.
            1. Uses manifest. 
        
    1. Push Notifications. 
        1. Push content to your subscribers and notify them. Complicated but a lot of resources. 
    1. Messaging stuff..... 
1. Why?
    1. Twitter lite case study. 
        1. Decided to redesign native app. 
        1. Less space than native app. (possibly good reason for us.)
    1. Forbes Case study. 
        1. Saw 43% increase in visitors. 
1. Support
    1. Google and Microsoft are service worker friendly. 
    2. Apple not so much yet. 

1. Chrome debug tools -> Application 
1. Updating a single file in the cache needs a complete cache rename. 
    1. Incremental caches. 
1. Need to clone response and the netwrok fetch because once consumed the memory is done. 

1. Things to checkout 
    1. Lighthouse
    1. workboxJs
    1. PWA builder
    1. offline-cookbook

1. Capital City Brewing Company. 