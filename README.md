[<img src="./img/playstore.png" height="52">](https://play.google.com/store/apps/details?id=com.rynop.clipguard)
[<img src="./img/appstore.svg"  height="52">](https://itunes.apple.com/us/app/clipguard/id1450439113?ls=1&mt=8)

## What is this?

An app aiming to protect video interviews while empowering viewers to authenticate said video.

Editing video is normal and typically honest. However nefarious editors may modify videos in post-production (editing/clipping/re-ordering) to push an agenda or change a narrative.

The quickest way to understand the problem being solved AND how it works is to read [this blog](https://rynop.com/2019/02/25/clipguard-app-to-protect-and-authenticate-video-interviews/) or watch this video:

<iframe style="display: block; margin: 0 auto;" width="560" height="315" src="https://www.youtube.com/embed/QUHjjNWz4gc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

QR code in video above can be found [here](https://github.com/rynop/clipguard/blob/master/img/demo1QR.png).

## How does it work?

An interviewee places a phone in frame, with the ClipGuard app running. The app displays:

- A timer that counts up every 1s. This exposes editing and re-ordering.
- A bar chart with data points (ever second) created by a [Pseudorandom number generator](https://en.wikipedia.org/wiki/Pseudorandom_number_generator) (PRNG). These data points make it harder for post-production replication of app AND give authentication to the sequence after the video airs.

**After airing**, interviewee shares a QR code. This QR code can be scanned in the ClipGuard app (by viewers of the interview) to reproduce exactly the same sequence, at the same time, as when the interview occurred.

## Who does this help?

Admittedly this app is only useful for a handful of people. I wanted to tackle an unsolved problem for my 1st app. Thought this was a nerdy yet novel solution.

The Idea was inspired by Elon Musk's [60 minute interview](https://twitter.com/elonmusk/status/1072528643488972802). He's one person I could see this helping.

This may also be useful for legal depositions. Proteting both the prosicution and defense - authenticating the un-altered recording.

## Is this foolproof?

Nope. But re-producing will take some work and time. This is a deterrent, not a bullet proof method. However, I think it solves the problem. Disagree? Ideas to make it better? Open an [issue](https://github.com/rynop/clipguard/issues) or [holler at me (@RynoP)](https://twitter.com/rynop).

## Chart colors

I tried to use colors on the chart that are [color blind friendly](http://mkweb.bcgsc.ca/colorblind/). I wanted to display 6 bars (last 60s) but things got too cramped, especially on small phones.

## Ideas/Bugs?

Open an [issue](https://github.com/rynop/clipguard/issues)

## Credits

See [credits](./credits)
