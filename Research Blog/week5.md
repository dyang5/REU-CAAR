## Week 5

### <u>Day 29 (July 3rd)</u>

Week 5, Day 1

This is now the 5th week of the program, which is crazy to think! Today, we have an unofficial day off from the REU and my parents came to visit which was fun. After waking up later than normal, I went for a morning 50-lap swim. For lunch, I met up with my parents and we went to a Steakhouse, which was quite filling. After showing them my dorm, I split off and tried to get some research done.

The most frustrating part is that the code I've written on my Jupyter Notebook still does not run using a GPU -- even after my group gave me some suggestions and it looked like it might finally work, it just still doesn't. I asked my advisor about this but it looks like I may have to move on for the time being and prepare for the presentation instead from tomorrow onwards. This really sucks because I spent about a week writing the code but now I don't even get a chance to run it. I hope a workaround/fix will come soon.

For dinner, AB, LH, ML, SS, ZS, SK, and two other non REU-CAAR students went to "Board 'n Brew" to celebrate a birthday (not saying who for privacy concerns). We played some board games (the place is known for board games and food) and had a fun time with a large group which is always nice. Tomorrow is the 4th of July; I don't have any crazy plans but will probably get both meals with my parents who are in town for a few more days. Other than that, I will hopefully have a lot of the presentation done/a fix to my Jupyter problem, but the latter seems relatively unlikely.

### <u>Day 30 (July 4th)</u>

Week 5, Day 2

Another day off -- this time due to the 4th of July! After another 50 lap morning swim (the pools were packed today due to Masters Swimmers and families celebrating the 4th of July... I guess), I met up again with my parents. We went to a seafood restaurant for lunch before heading back to their hotel to get some work done. I talked to them a bunch about grad school applications, my research project and the challenges/next steps (also showing them some of our group's presentations), and got a CodeForces problem done all in a few hours time. It was definitely good to catch up and to share what I've been working on and thinking about. I started working a bit more on the presentation we're scheduled to have on July 6th. I'm still pretty bummed about the GPU problem and my code not running but that will have to wait -- we may have a group meeting with our advisor tomorrow night (pending her reply) and we will certainly have to present Thursday morning, so these tasks take precedence.

For dinner, my parents and I went to "China Buffet" (it turns out finding a restaurant open on July 4th is quite difficult), which was better than expected. Afterwards, I got dropped back off at my dorms. My parents are staying a night or two more before going to visit my brother at his camp on the East Coast, so they will be doing plenty of traveling these next few days.

Despite potential Fireworks and S'mores plans being floated around by AG (our grad program leader), both plans ended up fizzling out (though we may do S'mores another time next week). I had a chill 4-day weekend but it'll definitely be a busy day at research tomorrow with the presentation/meeting prep.

### <u>Day 31 (July 5th)</u>

Week 5 Day 3: Meeting Day?

- 8:30 - 9:00 AM: First day back from a four day weekend; I had to start it off with my typical morning swim. I really didn't feel like going today but my goal is to stay consistent with exercise and I did just that. Got 40 laps in at a relatively quick pace which was good as well. I was definitely shaking off some of that morning rust caused by our long 4-day weekend.

- 10:00 AM - 12:30 PM: My main goal for today was to prep for the meeting (scheduled for later tonight) and presentation (scheduled for tmrw morning) and to present our work/motivation coherently and efficiently. I spent the morning for one last attempt to get TensorFlow working with the Cluster's CPUs, once again to no avail. As a result, I decided it would just be better to wait out the 1-2 hour runtime and run the program locally using the CPU. After staying an extra thirty minutes in hopes that the program would finish, I left the program running in the room with the help of Caffeine and just hoped that nobody would take my computer (it is pretty safe since you have to scan into the room to get in).

- 1:15 - 4:00 PM: After lunch, the REU congregated in our main room for some free ice cream and math problems given by Bill. For the interested, they include "using two colors to color the cells of a 3x9 (3x8, 3x7, and later 3x6 as extensions), prove or disprove the fact that there will always be a rectangle with monochromatic endpoints."

After the ice cream session, we went back to our research room to get some work done. I found out that the program I had been running broke due to an error on the line after the classifier, meaning  had to run it all again. This was a bummer but another run and another hour and a half later, I had some results for the DeepFace classifier on the FairFace validation set. The gender accuracy was 65% and the race accuracy was 60.8%, which isn't as good as I would have hoped for. In comparison to XG's EfficientNetV2 model trained on FairFace's train (95% gender accuracy, 70% race), these accuracies aren't good either. However, it is important to note that the DeepFace classifier is not trained on FairFace, and may perform better when we use it in combination with YOLOv8 on diffusion-generated images. For now, I think I'll move on from the classifier and try to build on a differnt idea (the "linear head" approach -- we want to add the linear head we train using gradient descent and some loss functions to the text encoder and we think this process may lead to more fair image generation).

- 8:00 - 9:00 PM: Our meeting was supposed to be during this time, but our advisor is feeling really sick and could not make it. In this regard, I think our presentation tomorrow will be a bit more important (she will probably make it to this one) as it will serve both as an update to our advisor as well as a general invitation to the grad group for any interested students/suggestions to improve our project.

After research, I had mainly relaxed in preparation for our anticipated group meeting. After finding out that the meeting had been canceled, per my advisor's requests, I left an update to the Slack channel to the work I did this week. I also watched Suicide Squad along with SS, AB, and DS, before calling it a night. Hoping the meeting tomorrow goes well -- looking at it now, my parts are complete so I'm hoping my group finishes up and we have a sucessful presentation tomorrow.

### <u>Day 32 (July 6th)</u>

Week 5 Day 4: Group Grad Meeting

- 8:30 - 9:00 AM: Morning swim. Meant to get out early today because of the important group meeting later at 10, and I did. I got in 50 laps in just around 30 minutes, which is quite quick compared to my other efforts.

- 10:00 AM - 12:00 PM: Today was our all important group meeting with our advisor and her graduate students. After some early time concerns (we got pushed to start the meeting since the first planned speaker's microphone was not working, and SS somehow snoozed her 3 alarms for the first time in a few weeks and had to Zoom in for the presentation), we quickly got started. We went over some of our motivation/project goals, before diving into our methodology and the experiments we've worked on thus far, and concluding with future work and exploration. Overall, the reception to our presentation seemed positive, and our advisor (as well as a few graduate students) gave us a few important suggestions/points to think about, including reconsidering one of our fairness notions. In our approach, we consider "fairness loss" (which aims to get the confidence each person in an image is male to be near 0.5) and "confidence loss" (which aims to get each person distinctly male or female). An important point that was brought up is that in a picture of a hospital context, there could be 10 people, 5 doctors and 5 nurses. With our current fairness notion, if all 5 doctors were male and all 5 nurses were female, the general proportion would be 50-50 resulting in a "fair image," but our approach does not account for the fact that the gender among occupation groups is not fair at all. This is an important fact/scenario we will have to account for, and we had some discussions about how we can do so (we may combine our approach with another that "erases biased concepts from diffusion models"). Overall, it was quite nice to hear some feedback about the presentation and to more formally present it in front of a bigger audience. Our presentation was followed by another on Source Free Domain Adaptation (notes to be completed later).

- 1:00 - 3:00 PM: In the afternoon session, I spent most of my time decompressing from the (relatively) stressful/important morning meeting as well as trying to understand the work done in the aforementioned [https://arxiv.org/pdf/2303.07345.pdf](Erasing Concepts from Diffusion Models) paper, which SS is working on implementing/experimenting with. This paper may come up useful in combination with our other work, so I am hoping to finish thoroughly reading it tomorrow and to begin working on a new angle to our project.

- 3:00 - 4:00 PM: We had a talk by Associate Professor at UMD Dana Dachman-Soled on "Types of Cyber Security Attacks." The talk was explained at a high level which made it easier to follow than some of our previous talks, and so it was quite interesting overall. A goal of mine is to attend every talk in this program (and I've been on track thus far) -- lately, a lot of people have been skipping these talks but I personally think it's important to hear from different speakers in different areas to get a better sense of the work being done as well as hopefully learn some new things.

- 4:30 - 9:00 PM: Today was a Board Game Night! hosted by Bill for the REU. A number of people came, including SS, AZ, LH, ML, MA, PM, DS, SK, ZS, CL, XG, and AB (at least 2/3 of the program). We got free pizza and I played a bunch of board games, including but not limited to SET!, Dixit, Texas Hold 'Em, and Just One (a word guessing game). I noticed that I am a bit particular about how games are played (I prefer them to be a bit more orderly) and I got a few comments from others about that, but overall it was a fun time, and it was great that the REU organized this event.

This was an important but short day for research but a quite fun day overall.

