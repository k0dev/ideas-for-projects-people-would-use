# Ideas for Software that People Would Actually Use

Inspired by https://github.com/joereynolds/what-to-code.

These ideas, as far as I know, don't exist yet (or have done a poor job with SEO on Google). These are also ideas I desperately wish I could have tried at least once, meaning many others probably have as well. It's difficult to stay motivated coding or on a side project when you don't know if people will use it, or if your end goal is solving a solved problem. This list aims to fix that.

This list is already over 50 ideas, and will reach 100 by 2022. Stay tuned, as I have several hundred in my list (the majority of them patently ridiculous and not a good use of anyone's time to read).

Feel free to use these for a hackathon, side project, or hacklodge project -- I'd love to see them get built! They include apps, webapps, and chrome extensions. All I ask for is they are open source, credit is given to Aayush or Divide-By-0, and your repo + site link back to this list :)

## Funding

If I particularly like a certain quality of implementation and you fully deploy the project publicly, I can award free hosting and small cash prizes ($100). This is at my discretion so people don't game the system or feel cheated; the point is to build the project for the learning and self-satisfaction, not the grant -- the money is mostly just so it can continue to exist :). Total bounties given counter: 2. 

viaprize.com has generously agreed to gaurantee this funding ($100) for 10 of these ideas -- feel free to check their website for which specific ones.

## Contribution & pull requests

If you make any of these, please make them open source! 

If you want to be added to the list of people that have completed a project, Request a PR adding the project idea, your project's URL, and your repo's url to [CONTRIBUTORS.md](./CONTRIBUTORS.md), and edit the README to mark them done. I can help brainstorm relevant communities, and send the site through a small marketing flywheel that should hopefully get you your first users (still in beta though).

## Index

[All Software](#all-software)
- [Music](#Music)
- [Health](#Health)
- [Programming Tools](#Coding)
- [Family/Roommates](#Family-Roommates)
- [Politics](#Politics)
- [Image Processing](#Image-Processing)
- [Video Processing](#Video-Processing)
- [Research/School](#Research)
- [Text Processing/NLP](#Text-Processing)
- [Fun](#Fun)
- [Shopping](#Shopping)
- [Crypto](#Crypto)
- 
<a name="all-software"></a>

## All Software

<a name="Music"></a>
### Music
- A Chrome extension where you can put in a song or artist, and it finds friends who have listened to that artist/song (by # of occurrences in their public playlists).
   - This is surprisingly highly requested, see [thread 1](https://community.spotify.com/t5/Closed-Ideas/Social-See-Friends-who-also-listen-to-an-Artist/idi-p/4397516), [thread 2](https://community.spotify.com/t5/Closed-Ideas/Sort-By-Friends-Who-Listen-To-the-Same-Artists/idi-p/72047), and [thread 3](https://community.spotify.com/t5/Closed-Ideas/Social-Listenalike-but-for-friends/idi-p/5041383). 
   - As [@alexgurr](https://twitter.com/alexgurr) points out, you'll need a Chrome extension to hit the friends API endpoint on Spotify web, or Facebook login to use FaceBook friends
- A program that takes your spotify playlist and converts it to another one of remixes of the same songs, to get some variety. [DONE: See contributors.md]
- A program that takes your spotify playlist and converts it to a clean version with the same songs, and removes it if it can't find any. Used to be able to listen to my playlists in the car with my parents. [DONE: See contributors.md]
- A tinder for songs -- plays the most commented 10 seconds of a song on soundcloud, and adds it to a playlist if you like it. Inspired by Soundsieve (https://github.com/wilzh40/SoundSieve) which is unfortunately dead.
- Connect your spotify and visualize spotify data insights as plots. Existing apps show tables or list, but it's a small jump to display eyecandy plots instead, and will help with virality.
- An automatic music video creator from mp3. Upload any collection of videos, pictures, or a topic, that you want to autoalign. The app detects drumbeats or other features, and staggers the videos to transition at those times.
  - Could potentially also upload a 3d scene somehow, and randomly move around and show the field of view, but at a speed proportional to music energy and rotating only when beats hit. Perhaps to import the 3d scene, could be autogenerated from an image/set of images, or just a spot on google earth or something?
- Automatically nightcore songs and post them as YouTube compilations
- An audio recorder where you can tap to add a flag at any time -- you can attach a note if you want, but the purpose is that later you can quickly skip to that time and know something important is there.
  - Can do this for a timer app/song player also, not just an audio recorder.
- Kaggle for music production -- the site provides samples and teaches the general structure to layer them, then has a periodic competition to layer them to create the best beat [Note: Kenny Beats runs a similar competition but without the lessons].
- A plugin that just takes a piano melody and adds corresopnding drums and reverb and a beat and a chorus and everything just off those notes (like the [harmony7](https://mitadmissions.org/blogs/entry/we-made-a-website/) MIT web.lab app).
- Scrape a karaoke or music video from YouTube, matches the pitch to notes (FFT?), then makes bars at those pitches for you to hit, and overlays your current singing on top of it. Allows you to quickly train pitch like Yousician or Riyaz, but for any song. Can be used for live singing, singing covers at home, or singing lessons.
- Website that takes a video or movie, Shazam's all the songs or looks up sound tracks if they're public, and converts it to a Spotify playlist automatically.
- Little dancer: Use echo nest labs and FFT to sync a bunch of clips to a specific BPM or sequence of beats. Using some beat detector (likely also FFT), have a mini cheerleader or dancing figure synced to the beat in the bottom corner of your laptop.
- An app that chooses songs of a specific BPM from all your spotify liked and playlisted songs, for workouts
- An app that plays hype beats or just a simple beat behind a podcast, so when you run you can listen and stay on pace
- A better rap lyrics generator than basic [MCMC/RNN methods](https://www.reddit.com/r/hiphopheads/comments/acwky9/original_python_program_that_writes/); use GPT-Neo to generate reasonable distributions over next words, then re-weight GPT-3 probabilities over next words by hard-coded poetic heuristics, such as amount of internal rhyming to same syllable count on the previous line, alliteration, etc. 

<a name="Health"></a>
### Health
- Sleep tracker app that detects when you fall asleep. It then turns off your sleep podcast/asmr and makes sure you get as close to 8 hours as possible, and wakes you up in a light sleep state. Note that existing sleep cycle apps force a wakeup time, but time-to-sleep is often so inconsistent that chances are you won't be getting 8 hours.
- Patient radiology in your own hands: An app that lets you take your physicians radiology image (or a picture of it), generate the hotspots of bilaterally asymmetric places or ML-determined anomalies, then patient can ask them to double check those spots and comment on what it is. Inspired since radiologists eyes pause at the place where people have tumors, according to some studies -- being more intentional about this could be pretty innovative.
- A collection of all large scale health studies for foods, ranked on a single number line of toxicity with error bars. Can scrape correlation/p values and error bars directly from papers.
   - Resulting graphic should look like: https://cdn.vox-cdn.com/uploads/chorus_asset/file/3523382/Medical_studies-05.0.png
- Search portal where you put in a dish and it says what percent of online recipes of that dish have nuts, maybe by country too. Done by scraping recipes with country of origin to determine what to avoid when allergic people eat that cuisine, and create an intuition about what allergens and dishes to avoid for a certain culture of restraunt.
- A chrome extension that goes through an Instacart/Amazon Fresh cart and finds them on an ingredient website and scrapes the ingredients, and flags foods with user-specified bad ingredients: whether its nut allergies, seed oil aversion, or high frustose corn syrup. Various nutrition authors would certainly help market this, especially on Twitter.
- A spoon/other device that emits sweet odors without having sugar in the food, to inspire kids to eat more of their food without being unhealthy. Can be done via diffuser instead of spoon perhaps, or just via miracle berries every meal.
  - [This paper](http://scholar.google.com/scholar_lookup?&title=The%20handbook%20of%20multisensory%20processing&pages=69-83&publication_year=2004&author=Stevenson%2CRJ&author=Boakes%2CRA)  says "certain olfactory stimuli, such as vanilla, caramel, or strawberry aromas [can] give rise to the perception of sweetness in an otherwise tasteless solution. ([source](https://flavourjournal.biomedcentral.com/articles/10.1186/s13411-015-0040-2))".

<a name="Coding"></a>
### Programming Tools
- A lightweight create-react-app for ML apps. This starter app would compile on first clone and run React, Tornado, and SQLAlchemy (easiest to do with Parcel). Would be nice to have a 'yarn deploy' or something that does a one click deploy to GCP/AWS as well. Would be cool if starter apps were just email collectors, commonly the first stage of hype in a startup anyways.
- A debugger to catch bugs like two functions being the same and differing in inconsistent ways.
- Automatically track all the keyboard shortcuts/clicks you do within an editor, and suggest/generate keybindings and commands for your most inefficient workflows (an interactive way to practice forgotten yet useful vim shortcuts, for instance)

<a name="Family-Roommates"></a>
### Family/Roommates
- Remotely control your grandparents computer/phone with one link click that you can send them. It should be one-time and only work for a few minutes, so hackers can't exploit it in the future. Chrome Remote Desktop requires Google sign-in from the same account in both places, which is harder to pull off for 2 different people.
- Make an algorithm for a mounted camera that sends SMS notifications (perhaps if your roommate leaves dirty dishes?) based off  this [similar one](https://medium.com/@ageitgey/snagging-parking-spaces-with-mask-r-cnn-and-python-955f2231c400) for parking spaces.

<a name="Politics"></a>
### Politics
- Rate your own affinity towards topics and get a ranked list of candidates that most aligned based on the wiki grid, like a buzzfeed quiz for local candidates.
  - Prefer to make this automated by building a scraping service for all candidates on ballotpedia comparing state senators etc. and scraping their beliefs from their speeches on youtube transcripts or personal links or twitter etc. Can also train on the wikipedia grid of candidate beliefs/policy votes. 
  - Existing solutions are lacking: isidewith (only for presidential race), voteredge (ugly), ballotpedia (no side by side or issues grid).
- Given a county, it automatically scrapes candidates running for local office and analyzes their social medias/public statements to infer possible political stances. If this is not enough info on local leaders, it might require an embedding/LDA type approach to analyze their public profile.
 
<a name="Image-Processing"></a>
### Image Processing
- Automatically make photos look good by aligning edge detection with the rule of thirds. Perhaps as a Chrome extension that runs when you hit crop on a google photos image link?
- Take a picture of a wine stand, and recommend wines by rating to price ratio.
- An actually good online red eye fixer.
- Make app/Chrome extension/background integration to autotag Google Photos images with ongoing calendar events, so I can search for the event and see the photos from that. Useful for class notes (if all your classes are on your calendar) and generally increasing searchability of photos.

<a name="Video-Processing"></a>
### Video Processing
- Convert any youtube video to the trapezoid holographic projection (like [this](https://www.instructables.com/3D-Holograms-Using-Phone/)) by running depth perception AI on the video, and changing the depths that different pixels are at on different screens, so you see a depth modulated image on top of your screen, holographically, for any video!
- Animation Generator: AI labels each frame in a video with the contents in text (representation learning), then based on given labels, generate missing labels/coherent story, then generate an animation based on all those labels. Can deepfake style transfer all images to be the same style (idea inspired by Eden Bensaid).
- A dashcam that alerts you if someone is giving you a parking ticket when you're away. Bonus points if it tells the cop that you'll be back in just a minute.
- Auto Analyze Game Footage: A drone above a sports game keeps track of all the footage and then you infer the plays the opponent is making based on similarity of movement, so you can get the strategies of an arbitrary team. Can also do with phone cameras possibly.
- A hidden camera on a lapel that lets you record all poker hands at a casino then analyses them for you.
- Trippy Video Generator: A superresolution/style transfer model runs on each frame of a video independently, leading to a very raw flipbook-style animation. Perhaps generate a trippy video from a regular video. For instance, upresolutioning every frame, or recoloring each frame (or any other transformation) independently with an imperfect generative adversarial network to have disconnected images but a connected idea.
   - Note: This got built! See https://aimlabs.mit.edu/ > Stylish Videos!
- Fill in people's videos when their cameras are off. By using the speech to face paper in a browser extension, fill in other's inactive google hangouts/zoom logos with low bitrate moving bitmojis, and send yours as that when your camera is off. Cool research done at 5.3 (https://arxiv.org/pdf/1905.09773.pdf).
- Given a (lecture) video, edit it so that automatically speeds up during times where no actual lecture content is delivered (ex. an instructor talking about their dog), and slow down when content is dense (ex. slide full of equations which the lecturer is going through). Use both visual info (slides) and audio (what the lecturer is saying). Example use case: a student wants to watch a recorded lecture video in an optimal manner that maximizes learning in a shorter amount of time. 

<a name="Research"></a>
### Research/School/Ed-tech
- An extension where you could double click a citation # in a paper and it would automatically open the pdf from jstor or other 👀 sources.
- Make app that embeds paperswithcode.com implementations directly to test (not generally, but a select cool few ones).
- Tunemeet for cohort-based classes: It's known that cohort based learning is powerful. An extension students can get that drops a chat box in their window if they're watching the same video (class zoom recordings or OCW content to start) as another student at the same time. Can perhaps comment on specific timestamps in the video, or have a Khan Academy-style board for any video.
  - There are a number of proponents of cohort-based learning, including [Wes Kao](https://www.weskao.com/cohort-based-courses-articles) or [Forte Labs](https://fortelabs.co/blog/the-rise-of-cohort-based-courses/) that I'm sure would love to see this!
- A script to apply to all companies on Glassdoor with just your LinkedIn, and doublechecking its autogenerated answers to all questions with the user, before it batch autosubmits all of it. Will likely require some Selenium in Python. <a name="OCW"></a>
- A site like MIT OpenCourseWare, where every user has an account. Accounts are important so that the site gets accurate data on which courses people actually study, and if the learning materials for a course are sufficient or need further improvement. Consider adding features such as something to find others to self-study a class with. For a class, add different kinds of permissions for the user accounts, such as course admin, course teacher, TA, and contributor. For example, a contributor should be able to easily upload a document they worked on. and the TA should be able to see that this document has been submitted and edit the class-specific-webpage to have this document show up there. The point of this is to streamline contributions to a site like OCW, so that all the class webpages do not have to be manually added by OCW staff and can instead be updated by contributors. Think, Github but for classes on OCW.
- Piazza, a question-answer forum, does not allow downloading or archiving posts on the site. But many times, an instructor wants to make the Q/A from a previous class accessible as another learning resource, either to the next offering of the class or to self-study learners if the class materials are made free and openly accessible on a site such as MIT OpenCourseWare. Make a piazza-equivalent that allows archiving and downloading posts. It’s likely that Piazza does not allow this in order to increase the switching cost to another, similar service (can’t import the Q/A into another site).

<a name="###Text-Processing"></a>
### Text Processing/NLP
- A creative startup name finder powered by baby names. Find meanings for baby babes, and make a site where you can input keywords your startup is about, and it will print resulting baby names with meanings with the highest keyword overlap (or min distance in the word embedding space).
   - Inpsired by https://www.joinleelo.com/blog/how-we-came-up-with-the-name-leelo
- Another startup name generator - input 2+ keywords, then try all reasonable pairwise ship names till you reach an untaken name .com/.ai/.io/other top TLD
- Convert chat in messenger to lowercase automatically (for speech to text or bad autocorrect).
- Keyboard shortcut for automatically fixing spelling in Google Docs+.
- A chrome extension that adds the per ounce/unit price to Instacart the same way Amazon does
- App that finds old messenger chats you left on read or unread, or unfinished threads, so you can respond to them. Requires probably mapping the last few texts to a score of how likely it was to be the end of a conversation.
- Talk to an 'painting' and have it talk back. Speech-to-text on your voice, gpt-3 for conversation, tokkingheads/other deepfakes for the response. Like Harry Potter paintings.

<a name="Fun"></a>
### Fun
- A better smart time-based phone password lock. For instance, if the current time is AB:CD, the user can set their password as say, (A+B), (|C-D|), (A * B % 10), (D) or a general user-coded function, so it changes every minute. Existing solutions only allow rudimentary functions.
- Automatic haircut chooser -- input a picture, and based on aligning you to a celebrity with similar facial features, overlay celebrity hair on top of yours to find a new style or to show your barber.
- Automatically take a picture of your face and take cross ratios and edge detection/curve detection to determine best sunglasses based on face shape or similar celebrities, customized sunglasses.
- Wiki game with subreddits and sidebars.
- Nerve (like the movie) but to avoid the horror scenarios, all submitted new dares must be moderated for safety. Alternatively mix and match a reasonable list of locations and actions.
- An actually good Chrome extension to keep you off Facebook etc. Tracks how long you spend on degenerate sites, then when you go to Facebook etc, it says "On average, you think you'll spend 16 minutes, but you end up spending 31 minutes on this tab. How many minutes do you think you'll spend this time?" And at the end of that # of minutes, it makes the page black and white so you can continue to browse but it'll be slightly uncomfortable.
  - Can also do for apps on phone.
- Windows automatic unzipper. When something is downloaded, unzip it to its own folder then delete the original zip file (Macs do this already, but not Windows). [DONE: See contributors.md]
- Intersite with a live count of how many people are watching. OG Silicon Valley watchers will know what this means.
- AI for deep sea mining. Recently there's been a lot of new deep sea mapping data, and there's a wealth of minerals/new species to be found. Map a list of all existing known underwater species to location discovered, and then search to find the deepest parts of the ocean where nothing has been discovered yet.
- A bidding platform for radio ads, where corporations/clubs/people put their ads, and radio hosts play the highest paying ones and post the time and station and location. Once the site auto-verifies it with audio matching from tune-in + shazam type system, it automatically transfers revenue from radio station to radio hosts (can be done easily via crypto).
  - I think college radio stations (like MIT WMBR) would really like this and probably use it!
- A Twitter bot that tweets the opposite of what a Twitter thought leader influencer says, and is therefore just as insightful.
- Run analysis on which dance teams placed in what rank, in order to see correlation with show order that they performed in, at shows like the Desi Dance Network.

<a name="Shopping"></a>
### Shopping
- An Amazon price per ounce/count calculation that actually works all the time, and the equivalent for Instacart, Walmart, etc

<a name="Crypto"></a>
### Crypto
- Add an actually nice frontend to https://github.com/nulven/zk-message-board and have the first proof-of-concept anonymous group posting app powered by zero knowledge proofs
- [Not my ideas, but still excellent] The four ideas at the bottom of https://bitcoinmirror.org/ have not been created yet and are not technocally impossible, but could be the first trustless applications of Bitcoin on Ethereum!
