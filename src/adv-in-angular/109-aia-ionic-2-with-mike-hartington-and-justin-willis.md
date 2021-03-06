---
layout: layouts/post.njk
title: >
  109 AiA Ionic 2 with Mike Hartington and Justin Willis
date: 2016-09-08 06:00:22
episode_number: 109
duration: 43:14
audio_url: https://media.devchat.tv/adventures-in-angular/AiA109_Ionic_2_with_Mike_Hartington_and_Justin_Willis.mp3
podcast: adv-in-angular
tags:
  - adv_in_angular
  - podcast
---

# [Angular Bootcamp](https://angularbootcamp.com/)

# [Angular Remote Conference](https://allremoteconfs.com/angular-2016)

Panel: Joe Eames, John Papa, Jules Kramer, Lucas Reubelki, and Charles Max Wood1:50 - Introducing Mike Hartington and Justin Willis

- [Mike’s Github](https://github.com/mhartington)
- [Mike’s Blog](https://mhartington.io/)
- [Mike’s Twitter](https://twitter.com/mhartington?ref_src=twsrc%5Egoogle%7Ctwcamp%5Eserp%7Ctwgr%5Eauthor)
- [Justin’s Twitter](https://twitter.com/justinwillis96)
- [Justin’s Github](https://github.com/jgw96)
  3:00 - Updates to Ionic Creator5:00 - Choosing between Ionic 1 or Ionic 29:15 - Updating Ionic with Angular’s changes11:25 - Using Ionic CLI to create projects13:00 - Overlap between Angular CLI and Ionic CLI15:20 - Progressive web apps vs Ionic18:35 - Ionic with PWA’s and Ionic with Cordova20:05 - What is a PWA?22:30 - Dispelling the rumors around Ionic and Cordova
- [Untappd](https://untappd.com/) social drinking app
- [Sworkit](https://sworkit.com/) workout app
  24:50 - Gaming and Ionic26:15 - Lessons learned from beta testing Angular 229:15 - Limitations to Cordova31:10 - Coding and Platform34:50 - Using RXJS and Promises36:50 - Animations37:40 - Testing Story for Ionic

### **Picks:**

[Ionic extension for VS Code](https://blogs.msdn.microsoft.com/visualstudio/2016/03/30/build-ionic-apps-in-minutes-with-vs-code/) (John)Gene Wilder and [_Young Frankenstein_](https://www.imdb.com/title/tt0072431/) (Joe) [ServiceWorker Cookbook](https://serviceworke.rs/)(Justin)[Reddit DIY](https://www.reddit.com/r/DIY/) (Mike)

### Transcript

Charles: Hey everybody and welcome to Episode 109 of the Adventures in Angular show, this week on our panel we have Joe Eames.

Joe: Hey everybody.

Charles: John Papa.

John: Hello.

Charles: Jules Kramer.

Jules: Hello.

Charles: Lucas Reubelki.

Lucas: Holla.

Charles: I'm Charles Max Wood from Devchat.tv, go check out angularremoteconf.com for three days of awesome Angular stuff online. We have two special guests this week. We have Mike Hartington.

Mike: Hello.

Charles: And Justin Willis.

Justin: Hey everyone.

Charles: Do you two wanna introduce yourselves?

Mike: Sure. Justine, why don’t you go first?

Justin: Sure. I’m a support engineer at Ionic. If you’ve ever been on our GitHub, we’re coming to possibly even Slack or even on Twitter, I’m constantly out there in the Ionic community. I also have been doing a lot of progressive web app stuff with Ionic lately. That’s pretty much what I do.

Mike: I’m Mike, developer on the framework. Basically, I do the same thing out there constantly in touch with our community. I also do some real work on the side.

Charles: Real work, that doesn’t sound like fun

Justin: If I can just jump in here real just quick because I don’t know if Michael talks about some other stuff that he’s done but he actually did a series on Naked that was pretty awesome, just saying.

Joe: If you got 10 minutes to watch, it’s a nice little intro.

Justin: True story, bro.

Charles: So we had Mike and Matt whose, I think he’s the founder or something like that of Ionic.

Mike: Yeah Matt is the lead on Ionic creator.

Charles: We talked about Ionic then and Ionic creator, do you wanna fill us in on what’s new in Ionic since October of last year?

Mike: Yeah, sure. Since last year, oh God this is going to be a lot of stuff, we basically have been heads down on Ionic 2.0 and working really hard at getting everything finalized and building out the framework, that way it’s taking advantage of all the fancy new stuff that Angular 2.0 offers and that we have with new tooling systems that are out there.

Joe: What does Ionic 2.0 have to offer? That’s the question, Mike.

Mike: It has a lot to offer. Basically when we decided to work on Ionic 2.0, we took everything that we had with Ionic 1.0 and went back and said, how can we make this easier, how can we make this faster, and how can we just overall improve everything, ten, twenty times? We’ve gone back and simplified all the code and structure, simplified all the components and just spent so much time trying to make Ionic even simpler than it was in version one.

Joe: Keep going. Details man, details

Mike: A lot of it comes down to taking advantage of all typescript stuff, taking advantage of all of the new built details that we have coming down with Angular and the ahead of time compiler that we’re currently working on and even going as far as to take advantage and start getting setup for some of the progressive web app stuff that we really want to take advantage of as well. Justin can talk a little bit more about the progressive web app stuff as well.

Lucas: Can we get that high level overview real quick of we know what Ionic is, most of our listeners do. But if they’re choosing today, I think we’re at a weird point where we have to choose between Ionic 1.0 or 2.0 How should people make that decision right now?

Justin: That decision is really important. If you have a project that needs to be done in two to three weeks, a month and a half, maybe consider sticking with Ionic 1.0 because it’s out there, it’s stable, well tested. But if you have a brand new project not due for any immediate future, maybe consider taking a look into Ionic 2.0 and start working with Angular 2.0 as well.

Lucas: If I’ve got something that’s going to be delivered because podcasting, people watching, recording by October-ish, I don’t want to put word in your mouth. I probably want to stick with Ionic 1.0. But if it’s something that might deliver after that, then you’d say go with Ionic 2.0. Is that what I’m hearing?

Mike: It kind of depends on the app. If it’s a very, very complicated app, you might want to consider sticking with Ionic 1.0 at least. But if it’s a rather straight forward app and you don’t have to do a whole lot of work, take Ionic 2.0 into consideration.

Lucas: Okay. It’s good to know. If somebody wanted to get started with one of these right now, if you don’t know either one of them, is it easy to learn Ionic 1.0 right now then go to Ionic 2.0 or somebody just jump right to Ionic 2.0 or what does that look like?

Justin: I had an interesting point, I knew Ionic 1.0 really, really well and then I started jumping into the Ionic 2.0 stuff a little bit after it had been developed. It’s pretty straight forward. If you know Ionic 1.0, you should be able to pick up the new APIs and the new components rather easily. Many of the components we had in Ionic 1.0 are still there in Ionic 2.0 and similarly with the APIs.

Lucas: Okay so it’s basically if I want to do this and I want to go to Ionic 2.0, I’m just going to use Angular 2.0 typescript and components versus Ionic 1.0 or I’m gonna use Angular one and the older style of technology, right?

Justin: Right.

Joe: I’m gonna ask you this, I'm in the middle of some Ionic projects right now and the first thing I realized is that we’re using Ionic 1.0, cause we are delivering right away, and we wanna get it out there and it’s live but soon as I did NPM install for Ionic, I got Ionic 2.0.

Mike: It’s kind of a tale of naming woes on our part. No one would suspect that power would have gone away so quickly. The actual global install of Ionic, that is the CLI. Then, the actual package name for Ionic is Ionic-Angular. It’s the kind of thing that we hear quite often.

Joe: Ionic 2.0 or Ionic 1.0.0? The CLI is just called Ionic, I got that. But if I’m using Angular 1.0, should I be using the Ionic CLI that’s called Ionic that’s version two or the one that’s 1.7?

Mike: No, you should be using Ionic 2.0. The CLI for Ionic 2.0.

Joe: It’s okay to build an Ionic 1.0 app using the Ionic 2.0 NPM CLI.

Justin: Right. It has all the same functionality to work with both projects and it knows if you’re in a V1 project or in a V2 project and it’s able to adjust accordingly.

Joe: Awesome. Then the actual MPM package I use that gets packaged with my project is the Ionic-Angular and that’s got versions for 1.0 and for version 2.0?

Mike: Correct.

Joe: Okay. I just want to make sure that’s clear because that confused our team when we got into it. We’re doing Angular 1.0 with Ionic 1.0 to deliver but we used the CLI for 2.0 which was weird at first

Justin: The CLI—I think one of the big important things was that it should have compatibility to switch back and forth. That part is kind of, it really changed the name of the most popular CLI package that we have. We just kept it like that and we named the actual framework version of it, Ionic-Angular.

Charles: My understanding was that Ionic 2.0 was kind of centered around Angular 2.0. Is that correct?

Justin: Yeah.

Charles: With all the RCs and changes that have come and gone, how much work have you all had to do to keep up with it and what has been the experience with Ionic 2.0 as things have moved from one to the other?

Mike: Very early on, it was quite a process to keep going with all the betas and all the alphas because they were coming out every other day it seemed. But as things stabilized on the Angular front, the upgrades have been kind of easier each time so going from RC 3 to RC 4 wasn’t too big of a change and sticking with all the RCs in the later betas has been a pretty easy upgrade.

A lot of the internal changes, while that may take a little bit for us, we’ve been working hard to make sure that any changes that our users will have to work with between Angular RC 4 or RC 5 even, we’re trying to make sure that those changes are very minimal, at least some on the user’s front. That way, they have an easier time to upgrade and we can just handle all the hard parts.

Charles: Does that mean you obstruct away some of the Angular stuff in Ionic?

Mike: Yes. Some of the Angular bits got chucked away because we just want to make sure that we have all of Ionic taken care of and injected ready in the whole bootstrapping process. I think a good example is our Ionic bootstrap that handles all of the injecting Ionic, all the animation, all the gestures so that way users would just operate Ionic bootstrap, that has the name of the root component that they want to initialize and everything else just happens magically.

Lucas: I want to talk about something that I think is just fascinating that you guys do and it’s something I’d love to see more teams do. I’m obviously a big fan of Ionic and both of Angular. Something I really loved you guys did is this Ionic CLI. You can actually create your own project very simply. What this does is it allows people who know very little about the app or the technology but may want to get into it to run the CLI and just run for example Ionic start foo and you get a project. It’s not only a CLI to run the app but it also generates and creates projects and can get you off the ground running and you can surf things with that CLI.

I’m curious, why do you guys go with this route? There’s a couple of places that do that out there but that’s not a common place yet out in the industry. What led you to do this?

Mike: Just ease of development, if our users have to read 50 pages of documentations or have step one sell this, step two make a directory, step three create all these files, here’s the package you're assigned, we’ve already lost them. At that point, they’re not really focused, they’re having to learn other things that aren’t Ionic. With the CLI and having all those scuffled out, they can start a project and just get up and running under a minute.

Joe: How much overlap is there with the Ionic 2.0 CLI which is really the same as the 1.0 I guest but you just put -V2 and stuff. How much overlap is there with that and the working with the Angular 2.0 CLI that they’re building?

Mike: Right now, there isn’t really any overlap, I think Justin, you know more in the Angular CLI than I do.

Justin: Sure, yeah. There are similarities with the Angular CLI where you can use it to generate components and components pipes. The Ionic CLI can also do the same. It’s something I hear a lot of praise whereas you can do Ionic generates pages and then whatever you want the page name to be. It will go ahead and generate you an Ionic page that’s ready to go with all the SAS files, the typescript file, and the HTML file out of the box.

Beyond that at this point, there’s not really too much overlap with the Angular CLI and the Ionic CLI.

Lucas: Do you see that in the future? I understand right now because the speed of development is probably not overlapping much but do you see this being something where the Ionic 1.0 piggy backs the Angular 1.0 or do you see this being separate or would the Ionic 1.0 create a blueprint for the Angular CLI which I believe is coming in the future?

Justin: I don’t really see much over lap between. It is Angular, Ionic is Angular and Angular is Angular but there are a few key differences between the two. I don’t really see any piggy backing going on between the Angular CLI and the Ionic CLI.

I’m sure there will be some more features that are the same. Like I said, the generate commands, that’s kind of a same feature between the two. There may be some more features coming out of the Angular CLI, especially once they get further with their web pack build that they are changing to, that may be similar. I don’t really see much piggy back going on or anything with that.

Joe: Who knows, we’re horrible at telling the future, maybe three or four months from now, we’re all piggy backing on the Angular’s CLI.

Charles: That’s what the Angular team always says, we’re terrible at telling the future, we’re not going to tell you when stuff comes out.

John: It’s the safest thing to do.

Jules: That’s how it rolls when you run a product.

Charles: Doesn’t make things seem better.

John: A couple of years ago, we had this world where companies were deciding between do I build a Native app or do I build a Cordova based app which today, one of the leaders in Cordova is Ionic, congratulations you guys there, not the only player in the game but you’re one of the leaders.

But now, we have other things too, we have things that are, I don’t know what category is that but you write C Sharp or Java and you end up with the Native app. Things like the C Sharp side as you write Zamron but you write C Sharp and end up with the Native application. But then one level down the scales, let’s say I know JavaScript but I still want a Native app and Ionic doesn’t appeal to me because you’re creating a Cordova app and maybe I’ve got some taste in my mouth as some executive that I don’t like Cordova which we should talk about.

An option I could do is I could write either React Native and get a Native app or could write Native Scripts with JavaScript and Angular and get a Native app or I could choose the Ionic route and go Ionic 2.0 and write it with Cordova. The fifth option we could do is progressive web apps and I know that you guys play in a couple those ponds.

Joe: Don’t forget Electron.

John: Electron ain’t gonna run on my phone thought, at least not today. Where do you guys play in those and why?

Mike: They’re all great technologies and I don’t want to say anything negative about them because if you’re C Sharp Shop or you’re C Sharp developer, it doesn’t make sense to you to try to relearn, to learn JavaScript and learn all that. Might as well just use Zamron, they all appeal to different kind of developers.

If you are comfortable with more of a Native background, some of those projects, make sense if you’re comfortable with that and you are okay in diving into some Objective C or Swift or even some Java for whatever reasons.

That’s fine. I don’t see anything wrong with them. Ionic and Cordova have this nice little user group where these people who are the web developers, people who don’t really predict what you want to know, Objective C or Swift or don’t want to write it and don’t wanna deal with Java and just wanna stick with DOM, they want to stick with HTML, CSS, JavaScript and that’s where they’re comfortable at.

Joe: Is that what you see people coming to you for, is that the developer persona basically? If you’re a web developer you like Ionic, is that kind of where your target has been?

Mike: Yeah, that has been our target from a sales standpoint. It’s a big user group that doesn’t get a whole lot of attention. People who are traditional, I know JavaScript, CSS, I messed with Jay Gray back in the day and that’s where our user group rise.

Joe: In the progressive web app versus Ionic, not really versus but, we can define what progressive web apps are, I’ll let you guys go there if you want. I know that there’s been some recent developments with Ionic and PWAs and Ionic with Cordova, can you explain the difference between those two? Why you’re planning in both those areas?

Mike: Yeah. Justin, this is your type of thing.

Justin: With Ionic 2.0 especially, I would just like to say, you could build a PWA with that Ionic 1.0.0 and it will work, great out of the box and all that good stuff. But with Ionic 2.0, we are working on making a progressive web app, like a first set standing right next to Cordova.

The cool thing about Ionic is since we are based on web technologies, we are purely web, that same app that runs Cordova on your phone will 95% of the way work just as good as a PWA or even Electron way in the future.

That gives Ionic developers, you can deploy your app for cross Cordova, you can apply us a separate web app and all this, anything else that the web runs on, you can pretty much deploy an Ionic 2.0 app too.

With progressive web apps, you get a lot of the low entry to users. Instead of a user having to pull up the app store, download an app and then open the app and actually get that functionality, if you decide to deploy your Ionic 2.0 app as a PWA, they simply open up a URL and then boom there is the app, it’s ready to go. They don’t even really have to install it to their home screen if they don’t want to.

Joe: Can you explain a little bit what a PWA is and where they came from? Because they seem to come out of nowhere last year.

Justin: Sure.&nbsp; A progressive web app is a web app that is using a lot of new technologies that have come out in the past few years to make them more app like. Along with some of the things that browsers are doing now, allow those apps to be added to the home screen of your phone and sit right next to all of the native app that you have installed on your phone.

Progressive web, you basically write a web app and you give it a service worker, you give the manifest object some file. With those two things, that gives you offline capabilities that native apps have had for years and years but with your web app instead, and the manifest basically just tells the browser like, “Hey, I want the user to add it to the home screen and here’s my icon for that.”

That way it, to the user, it appear to just be any normal app that they would put on their phone but it’s with all of the benefit that come along with like I said before, just being able to visit the URL and there’s your app and all that good stuff.

Joe: Limited device features integration right now is poured on Native devices but it’s growing fast.

Justin: Yes.

Mike: It’s going really fast. Most of the core functionality that is available in Cordova is starting to become available inside of a browser. Things like file access, camera inputs, all of that is slowly becoming available to these evergreen browsers that we have out there.

Justin: Yeah, and with Chrome I would just like to add, the support for all these APIs are increasingly becoming available very fast, service worker is way more supported now than just a couple months ago.

Things like vibration API, being able to get user video to get access to the camera. Most of your big browsers like Chrome, Firefox, Edge, Opera, and even Safari, there’s a lot of those APIs that are already available. With all the new APIs coming on the shoot, I see it a couple of years being able to do almost just as much functionality with your web app as you can with a Native app.

Joe: If I wanna do more native type features, that’s when I jump from PWA way up to Ionic with Cordova, right? Dispel the rumors now, let’s play personas, let’s pretend I'm some C level executive and I’m looking at whether Cordova is bad, is it too risky for proposition, you get slow apps or just not as good as Native, why would I bet Ionic and tell me why I’m wrong?

Justin: Those kind of negative ideas that Cordova has may have come from two, three years ago or so. Back in the early days when we were still dealing with frameworks that weren’t focused on performance, we were having to kind of like take this plugin and this UI component and make this together and maybe we had backbones somewhere in there because we needed some kind of way to have some kind of models where Ionic, chance is that we take care of all of the hard stuffs, all of the performance issues, all the animations. We make all that easy.

Charles: I have a question, I’m curious, it seems like since Ionic has been around for a while, there are probably apps out there that people have used that they may not realize have been written in Ionic. Are there some good examples out there that give people an idea of what Ionic is capable of and also possibly help dispel some of the uncertainty around Ionic and Cordova that John brought up a minute ago?

Mike: I have two apps that right off the bat I know. So far my favorite, not even like Ionic app but just my favorite app in general, Untappd, because I love, it’s basically a social network for beer. You check in what kind of beer, you can post it, share to all the social medias that are out there. They recently just rebuilt as an Ionic app, they have a big user base.

Another one is Sworkit, it’s been featured on both the Google Play Store and iOS App Store as one of the top apps. Last time I chatted with them, I think they were up to 12 million downloads. 12 million people can’t be wrong about an app.

Charles: The other question I have is can you write things like games in Ionic with some of the games out there?

Mike: You could, theoretically. If you use things like Faizer, it’s possible. But depending on the game that you want to write, it may just not make sense to use web technology for that. There are very specialized APIs that take advantage of all the hardware specific features that iOS and Android has. But it just makes more sense to do it more in that.

Jules: I have a question and a comment actually. My comment, I don’t know that a lot of people who are listening probably know this but I’ve mentioned it in a couple of keynotes that Ionic is probably, has been our first beta tester for Angular 2.0. Ionic continues to be one the themes that we go to for every single one of our releases to validate our release before we actually release it to the public.

I wanted to say thank you because I’m sure that that is not an easy thing to do at our pace of release and sometimes we probably mess with the dates a little bit on you guys so thank you for all the hard work you guys do, just trying to be polite.

Mike: Thank you for including us in that whole process. I know Adam really appreciates it.

Jules: I just wondered if there’s things that you’ve learned from being part of that process that affected how you created Angular and I thought a lot about bringing up this topic and asking this question. I’m ready for the good and the bad because I think it’s really cool that you guys work so closely with our engineering team and we rely on you so much to validate what we’re doing here.

Justin: Can you just repeat that again?

Jules: I’m just curious if there may or there may not be, you guys might not be involved in that part of it, I don’t know. I was just curious by being involved in the whole, I think you guys were the very first testers we had for Angular 2.0. If being involved with so closely through this whole development process has given you, it might not be the things you learned regarding Angular or Ionic but just things you’ve learned about maybe the release process or building software, anything that I don’t know. You may not have any comments, though.

Justin: The change log is always important and do not forget that change log ever. Always be vocal about things that you changed, things that you’d appreciate and things that you just don’t want users to use. Fail very loudly.

Jules: Fail loudly and fail fast.

Justin: Yeah, fail very fast and rely on the tooling, that’ll help you out more than just clever code.

Jules: Nice, but again, thank you cause I’m sure that’s taken lots of your guys’ engineering time that could’ve been used elsewhere and we totally appreciate you and everything you do.

Justin: It’s been great because we’ve had a chance to learn Angular 2.0 as it’s being built and seeing some of the internal decision making and seeing how that whole process works out, it’s just been very beneficial to be part of that.

Mike: As an Angular fan boy, probably here, I’m a proud Angular fan boy, joining Ionic and being able to see, I get a lot of details how Angular works internally and from the engineering side and all that stuff has been really cool.

John: From the application developer community, the effect is you create these kinds of pressure on the product that benefit us. The fact that the Angular team has been turning to you for all this time and getting your feedback, the rest of us just kick back and enjoy, we don’t have to rely strictly on the Angular team’s own wisdom and own experience. We’re all grateful to you, not just the Angular team.

Mike: Giving back to the community and everyone helping everyone else.

Lucas: In the time that we’ve doing this podcast here, I can’t tell how many minutes we’ve been on but I went in and I installed on our fresh machine, I installed all the tools following your start up for Ionic and ran it in the web browser and ran it in my iOS simulator. I can’t imagine it’s been more than twenty minutes here but it was, help me take my time and ask some question as I went along, and it’s pretty good, I didn’t render a single glitch so kudos to you on that too.

Mike: Yay, that’s really good to hear.

Justin: Yay, I can sleep tonight now.

Joe: Wait wait, there’s smoke coming out of my Mac, is that right?

Justin: That’s gotta be a Java update. That’s not us, that’s certainly Java’s fault, we always blame that.

Joe: Lucas had a question earlier which he was trying to get in there. Lucas, do you want to ask that one about Native Script?

Lucas: Well I think, more so, I wanted to just know, I think you’re constrained by the limitations of Cordova at the end of the day. Following the history of Cordova as it knows phone gap and it got bought by Adobe and wondering what Adobe’s going to do to Cordova and phone gap seems to waiver bit. If you run into hard limitations with Cordova itself, okay we love to do more stuff but unfortunately Cordova just is not givinig us what we need. Are there limitations to that passive, the playground that you live in?

Mike: For the most part, the only limitations that I’ve really seen don’t fall on Cordova, oddly enough. A lot of the bottle necks that we have seen had been does the browser supported, is this something that’s fitting to run in the browser or in a web view, do the native operating system actually have support for this?

Something that people could easily look over, keyboards. Being able to handle working with a keyboard and trying to adjust your layout. With iOS, that’s totally no problem. They report everything as you expect in a reliable manner. But on Android, we’re not getting consistent keyboard size reads, the events come in in a weird order. Just because there’s so many keyboards that could be out there. Those have been bottleneck, dealing with the operating system and dealing with some of those things. But as times gone on, we’ve seen the browser catch up and take care of all those issues.

Joe: Do you mind if I ask some coding questions about the apps that you guys are building with Ionic?

Mike: Sure.

Joe: I’m looking at some sample apps, I'm specifically talking about Ionic 2.0&nbsp; and looking at the cute puppy pics for example that people can download. Let’s see sample app, just so people know I didn’t make that app.

Mike: It’s an app full of Corgis.

Joe: Yeah, it’s not my side passion. But inside this app, for example I’m looking here at the app folder and you’ve got an app component, some tabs, home and all that fun stuff. How hard has it been for you guys to keep up with the pace that the Angular team is moving at, cause it has been moving fast as it gets close to release. If I know Angular 2.0, how different is it developing for Ionic in here? I’m looking at the code that I’m staring at here.

Justin: It’s not very much different. I think one of the few things that we changed is we have our own custom bootstrapping method and that’s just to make sure that our gestures, animations, and all of our components get bootstrapped, get substantiated before the actual app does and handle all of that differences. Once you get past that, you’re writing Angular components, you can use everything that act component has available to it, you're writing raw typescript and you’re just taking advantage of our, I guess we just call them injectables now, no longer provide us services. All of our injectables and all of our classes like app controller and all the components like Ion tabs.

Joe: Like I see here in your route components which is called my app in this thing, you’ve got a custom bootstrap called Ionic bootstrap, is that the thing that you’re talking about, the custom version of it?

Mike: Yup, that’s the custom bootstrapping logic.

Joe: I see here you’re pulling things out of the Ionic Angular module in your graphing platform. What does platform give you, cause that’s not an Angular thing, that’s an Ionic thing.

Mike: Platform handles a lot of the Cordova specific stuff. There’s an event in Cordova called platform.ready or a device ready for Cordova. Basically, when that kind of bridge between the upgrading system and the web view is made, and you want to call Native functionality on the camera or creating sequel data base, you want to make sure that all of that’s done after platform.ready.

We have our platform.ready which handles the device ready events, also handles when the app goes into the background. If you want to register a custom action for the Android’s hardware back button. It does quite a few things but it sits on top of what Cordova already does then we just make it a promise instead of call backs, make it easy for developers to use.

Joe: What’s cool about this for people who haven’t tried it yet, if you’re inside with Angular 2.0, this isn’t really Ionic but it’s Angular 2.0 I guess, using ES 6 modules. If I’m in the typescript inside your class and I want to find out what’s available inside the Ionic Native library, I can just use Intellisense trying to figure out, okay I see a status bar but is there any accelerometer? Is there any battery status? I don’t have to go hunting and packing to the docks, I can use Intellisense to do those things.

You mentioned really good things, I want to ask a good question about that. You said you’re using promises for platform ready, there’s been a big push for the Angular world to use RXJS. Is that something that’s also going to be an option? Or are you guys leaning towards a promise side or is there a mixture?

Mike: There’s definitely a mixture. It comes down to use whatever is right for the situation. I think a better example of the way we can see this is inside of Ionic Native. For things like the camera functionality, we have a method called camera.get picture and then it can instead of it returning miserable, it just returns a promise because it’s just going to execute that one time and either return a success or a fail.

It doesn’t need to be an observable that can return multiple values over time, it just returns that one instance. Something like geo location where you can get location and watch the geo location as it changes, it’s gonna return that data as the geo location changes. That makes sense for an observable.

Lucas: You really have to pay attention to the API that you’re getting. From getting multiple values that you guys use to RX effects, what is observables and if I’m getting it to there is something very deterministic that has an end, I’m getting a picture of the camera, this isn’t going to be 90 pictures.

Mike: It make sense like in cases like in Bluetooth, it make so much sense if you want to call Bluetooth scan. You just return an observable because that could change multiple times or so. The Intellisense makes that easy though, it’ll let you know okay you’re going to get a picture or get a picture on the camera. You hear the options it takes and it returns a promise.

Joe: Awesome. Are you guys taking advantage of the Angular or Angular 2.0 animations yet or you guys have your own animations? How is that working?

Justin: We’re not taking advantage of the new NG animate yet, we do have our own internal animations which allows us to have a little bit more control over how views animate in. We’re also animating not just the individual components, but we’re animating the components, the internal nav bar, the nav bar titles, animating in that back button as the page comes in. We’re doing a lot of coordination and we just need a lot more control than what NG Animate offers at the moment. We were using had this out a couple of months ago and NG Animate was still under development.

Charles: What does the testing story for Ionic look like at this point?

Mike: Justin, do you have a good response for that?

Justin: At this point, I will happily admit that there’s not that clear of a testing story yet but I know there’s a lot of work going on right now.

Testing in general especially with Angular 2.0 is still an evolving story, no one really has all the answers yet. We’re all figuring it out as we go on and as frameworks mature, the testing rally becomes much more clear and everyone will have an agreed upon standard.

John: Bad testing, who cares

Joe: Oh gosh, don’t say that, John.

Justin: That’s my whole workshop, but Angular connect is on testing.

Joe: I care, I care, I know John cares too.

John: I do.

Mike: I like CSS, though. I’m not particularly focused on testing.

Joe: I only test my CSS, that’s the only thing I do test. It’s all automated, CSS testing. Just think about that for a minute before you want to clear your self.

Alright, we should wrap up, we had a couple of people have to drop off unexpectedly for various reasons. We’ll go through, John and I will have our picks and then you guys do your picks and we’ll end the show. John, how about you? What picks you got for us?

John: Sure. Obviously, Ionic and Angular are awesome but I’m going to pick something slightly different in the coding world.

I was playing around with VS code and an extension has existed for a while that I didn’t even know that I’m really excited now it exists and that is the icon extension for visual studio code. The reason I’m excited about this is that now, when you’re in that left panel, the explorer, the finder, the windows explorer, whatever you call it, the project view of your preview, they now have an extension to the VS code that you can pull down and show icons for HTML, typescripts, CSS, whatever.

I love that because it just make it super easy to see and identify files especially with Angular 2.0 when you’ve got three files named the same like home component TS, home component HTML, and home component CSS. Not only is the extension different but now you got a file icon next to each that makes it easier to pick and choose what you need. Definitely look into your extensions and go check that out, it’s free and it’s awesome

Joe: Okay, I’ve got just one pick that I’d like to go over, that is Gene Wilder. Gene Wilder died yesterday as we were recording this, I think that he’s just an amazing actor. Some of the best movies ever produced, he’s starred in. One of my favorites which I have probably seen at least a couple of hundred times, Young Frankenstein, one of my favorite movies of all time.

If you haven’t seen Young Frankenstein first, go see it, but I’m just going to pitch Wilder, a great actor, I’ll definitely miss him.

John: Yeah. Blazing Saddles, Stir Crazy, Willy Wonka, so many, Silver Street, great guy, he’s going to be a big loss.

Joe: Yup. Justin, how about you?

Justin: Because I’ve been so focused on progressive web apps lately, and service workers are a corner stone of that, but they seem to be hard to get into for a lot of developers or not really understood completely. There’s a Mozilla website called the service worker cook book. You can describe what HTTPS service, that will be www.rrke.rs and has huge examples about different things you can do with service workers, real code examples that you can literally copy and paste and it works out of the box which is the best docs in my opinion. It gives you a nice overview of all the different things you can do with service workers and how it works and all that stuff. I think you’re getting into progressive web apps, that’s definitely a good website to check out.

John: Awesome. Then, Mike?

Mike: My pick, I try to do especially, on the weekend, as little programing as possible and try to focus on other things. I have a sub Reddit called DIY, it’s full of awesome little projects that you can do. Some of them ranging from being these huge remodels of the entire bedroom and some of them just being I made a little shelf for my kitchen, totally something not technical related but breaks up being focused on code all the time and gives you another output for all your energy and focus, something I find really important.

Joe: Awesome. Well, thanks again guys for coming on the show, we’re always happy to talk about Ionic, great product and we will see everybody next week.

John: This is great guys, thanks a lot.

Mike: Thank you.

Joe: See you!
