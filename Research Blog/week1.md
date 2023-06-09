## Week 1

### <u>Day 1 (June 5th)</u>

Orientation and Introduction Day!
 - 11 AM - 12 PM: Bill Gasarch (program director) gave us a program overview and we learned about the other groups.
 My group members include SS, AF, and XG (initialed for privacy).
 - 1:30 - 4:00 PM: Met with Furong and Pan to discuss research goals for the summer. Since Furong is leaving for China in a few days, we laid out expectations for our project as well as started brainstorming ideas based on our group's interests and collective research experiences. Our preliminary ideas/thoughts include **concept-level fairness in LLMs** and **Fairness in Generative AI/Diffusion Models**.
 - 4:00 - 5:00 PM: Listened to Professor Victor Albert discuss the Quantum Error Computing Project

Socially, I ended up going to Target to get stuff for our suite, with one of program leaders and graduate students Auguste, along with SS, AZ, and AB. I then headed to the Gym to get a membership and play Raquetball with SS and AZ before heading to a late dinner with SS and AZ (after finding that the Student Union apparently closes at 4 PM).

### <u>Day 2 (June 6th)</u>

Literature Review (pt. 1)
 - 10 - 11:30 AM: We organized papers into categories, including Vision Language Models, Fairness (in Language Models), Group Fairness, and Generative Models, including GANs and Diffusion Models. After organizing our work, I spent most of the morning reading background about vision language models and the pioneer paper for GANs (Generated Adversarial Nets) to better understand the research context we hope to work on. As a group, we are hoping to work on fairness in the context of generative models such as diffusion.
 - 11:30 AM - 1:30 PM: Headed to get University of Maryland ID Cards and then lunch.
 - 1:30 - 3:00ish PM: Read more about Denoising Diffusion Probabilistic and Implicit Models (DDPM and DDIMs). These papers were a bit more dense/harder to read and understand but I found another resource to summarize major differences and similarities (my understanding is discussed below):
 
 > DDIMs are consistent-- i.e. starting with similar latent variables will yield to results with similar features -- whereas DDPMs are not, and DDIMs can run much faster than DDPMs as a series of Markov jumps (each of which can be modeled as Gaussian) can be modeled as a larger combination of Gaussians. On the other hand, DDPMs approximate the reverse diffusion process (from data to noise) and can run much slower.

 - 3:00 - 4:00 PM: We discussed a general research plan for what we want to work on this summer. I felt this discussion was fruitful -- we talked about a [Fair Diffusion Paper](https://arxiv.org/abs/2302.10893) that seems close to what we want to do, and possible extensions/limitations of that research and the scope of our work. Tomorrow, I'm hoping to continue reading this paper and another one a Grad Student shared as of 6:00 PM.

 - 4:00 - 5:00 PM: Listened to Auguste (AG, a grad student mentor for the Computational Geometry project as well as co-lead of the REU program) discuss the Computational Geometry project, including the Hilbert Metric, Voronoi Diagrams (whose dual is the Delaunay Triangulation), and the Delaunay Triangulation. I found it quite interesting how similar the project was to my Circle Packings project last summer, which you can find more about [here](https://github.com/dyang5/CirclePackingsResearch).

 After research hours, I went to Chick-Fil-A (CFA) in the Student Union with ML, DS, PM, and NL before heading to the gym with ML and DS. DS and I played tennis before heading back, and I ended up back in the dorm soon after, playing cards with AB. Later, we ended up playing cards with ML, DS, SS, JS, and PM, including Spoons, ERS, and Go Fish. Socially, I'm happy with how the REU is going but I want to keep making friends/being around people outside my suite and REU group as well. Though paper reading can be monotonous, I felt like the discussion about our project was fruitful and so today was overall a solid REU day.

 ### <u>Day 3 (June 7th)</u>

Literature Review (pt. 2)
 - 10 AM - 12 PM: We continued to read the [Fair Diffusion Paper](https://arxiv.org/abs/2302.10893) and [Debiasing VLM via Biased Prompts Paper](https://arxiv.org/pdf/2302.00070.pdf) that addresses biases implicit in text prompts. As of now, our project focus seems to be on fairness in diffusion models and generative AI, and so I anticipate that these papers will be the glue to our project. The main goal of my paper reading today was to understand and discuss the concepts of these papers and to think about potential avenues for exploration/extension as a group. We had a productive group discussion about the concepts in the first paper and what we might explore, namely situations where prompts have implicit biases. 
 
    The first example presented in the paper is "give a photo of the face of a firefighter." To address the explicit gender bias (`men` associated to the word `firefighter`), the paper proposes using a lookup table (mapping firefighter to the gender bias) and "guidance" (consisting of an emphasis on females and a de-emphasis on males) to adjust for this bias. We are curious how this work could be extended to implicit biases: for example, the prompt "give a photo of a hospital" might yield predominately male doctors.

- 1:30 - 4:00 PM: One of group members had to leave early, so that left us with me, SS, and AF. We began reading the second paper which attempts to address biases in text prompts (using orthogonal projections to create a projection matrix that essentially acts to project out biased directions) and thought about how that might apply to the work we're interested in. We also had more casual talks about research as a whole and previous/friends' research experiences. I'm quite happy with the communication and transparency we have in the group about the process as a whole (especially with SS and AF) and so I'm hoping this will lead to a solid research group and effort this summer.

- 4:00 - 5:00 PM: We listened to Bill Gasarch (program director) give his [Muffin Problem](https://www.cs.umd.edu/users/gasarch/MUFFINS/muffins.html) talk which was quite fun/informative. I asked Bill if he would be around at Swarthmore to advertise the REU (I was thinking of getting him to give the talk as well), but he said he wouldn't be back until the next year. Bummer -- I hope when I am older I can be as energetic as Bill is.

After research, I grabbed some Q-Doba (QD) from the Union, ate, and then headed back to the dorm with ML, AB, and LH. I talked about sports with DS for quite a while, "worked", and will probably end up playing board games later as well. Air quality was not great due to wildfires in Canada, so no outdoor activities for me today.

All in all, I'm happy with the direction my group is starting to work towards after just a few days of paper reading and meeting, and pretty pleased with the communication about the process/openness about my research group with regards to general social conversations and group expectations.

 ### <u>Day 4 (June 8th)</u>

Literature Review (pt. 3)
 - 10 AM - 12 PM: The air quality today was deemed Hazardous (200+ AQI) and so today was a work-from-home day in place of working at Iribe (IRB, or the CS/Engineering Building). This meant XG, a UMD student who is our fourth group member, didn't come to campus. SS, AF, and I found a place in the basement of our dorm to work. We continued reading the previously mentioned Fair Diffusion Paper, which I have been trying to read particularly carefully since it will seems very relevant to our intended project direction. SS shared with us a new [Debiasing Vision-Language Models with an Adversarial Classifier](https://www.semanticscholar.org/paper/A-Prompt-Array-Keeps-the-Bias-Away%3A-Debiasing-with-Berg-Hall/efabdd27929796b712cb1b3a3051ea5358dc1200) paper that uses an adversarial classifier AFTER a pre-trained VLM. 
 
    In comparison to the two previous Fair Diffusion and Debiasing papers, which affect the step immediately after the encoding of a text prompt, this paper influences the post-layer step. This gives us multiple possible avenues for exploration/extension in our own research process, and we will have to weigh the pros and cons of each approach a little more.

- 1:30 PM - 4:00 PM: After lunch, I discussed the research process a bit more with my group and moved on to reading a [Fairness and Debiasing Survey](https://www.semanticscholar.org/paper/Debiasing-Methods-for-Fairer-Neural-Models-in-and-A-Parraga-M%C3%B3re/7a1bf9474ae0cc07aa01d010449970a9ddf9baa5) which consists of a summary of relevant terms/written works/etc. in this subject area. Today was a slower work day due to the work-from-home nature, but those are to be expected on a long 10-week research program.

After research, I picked up a package from Queen Anne's before heading to the gym to play Raquetball and later Ping Pong with AF, SS, and ML. There was a whole ordeal where I thought I lost my key cards and went around searching for them, but it turned out that AF, who had gone to the gym early to get a membership, had somehow ended up putting both my lanyard and her lanyard on her neck. She mentioned that she felt that her lanyard (with keys and a ID card) felt heavier on the way to the gym afterwards and I can imagine why; all in all, I'm happy I didn't lose it -- while it was a bit stressful for 10 minutes, we laughed it off afterwards. Raquetball was quite fun and we alternated playing two 1v1 games, switching partners after each period of time. Then we had to play doubles ping-pong since the gym somehow has more than four paddles to borrow but just one ball total. Socially, I think I'm doing a good job mixing with the REU students but I'm hoping to talk more with people outside my suite/research group. 

Now that I'm looking back on it, it is a bit funny that my social review for the day ended up longer than my research recap. I guess that's part of the work-from-home lifestyle, but it's also partially due to the fact I was trying to understand the important papers a bit more closely. Looking forward to tomorrow, when the air quality is hopefully better.

### <u>Day 5 (June 9th)</u>

Literature Review (pt. 4)
 - 10 AM - 12 PM: The air quality was noticeably better today (it seems the bad air from the wildfire has traveled south), and so I headed to Iribe (IRB) to work with my group. The first paper to read was the Survey paper discussed above. Surveys are typically summaries of the work done in the field, and so they are naturally easier to read and follow. I reviewed definitions for fairness ("the absence of any prejudice or favoritism toward an individual or a group based on their inherent or acquired characteristics") and bias ("unintended behavior resulting from correlation-based processing that ignores further context not explicit in the data") in ML before reading and thinking about relevant group fairness metrics. 

To summarize the literature we've read so far using the language from the survey, we have considered both "distribution models" (consisting of strategies that modify the dataset distribution prior to training) -- as in the [Debiasing Vision-Language Models with an Adversarial Classifier](https://www.semanticscholar.org/paper/A-Prompt-Array-Keeps-the-Bias-Away%3A-Debiasing-with-Berg-Hall/efabdd27929796b712cb1b3a3051ea5358dc1200) paper -- and in "inferential models" (which intervene during inference time to make models fairer) -- as in the [Fair Diffusion Paper](https://arxiv.org/abs/2302.10893) and [Debiasing VLM via Biased Prompts Paper](https://arxiv.org/pdf/2302.00070.pdf) which use prompting and vector-space manipulation to reduce bias in vision-language models.

- 1:30 - 4:00 PM: After lunch and some free ice cream from Auguste, we went back to our work spot to finish up the Survey paper as well as start reading about CLIP (Contrastive Language-Image Pre-training). [CLIP](https://arxiv.org/pdf/2103.00020.pdf) is an incredibly important part of Vision-Language Models. In the papers we've read, we've seen it referred to as both an encoder and a classifier. CLIP is trained with a batch of N (image, text) pairs, to predict possible (image, text) pairings across a given batch. This is done using both an image encoder and text encoder to maximize the cosine similarity of the image and text embeddings of the N real pairs in the batch, and so it's an essential part of the text-image classification process. I didn't get to fully finish the paper, since I hit a bit of a Friday Funk, but I hope to finish this soon and to aggregate a bunch of my notes from this week into an Overleaf document for further discussion and presentation. My group is hoping to Zoom with our advisor sometime next week to get the project more sorted out and to hear any suggestions.

- 4:00 - 5:00 PM: Listened to Professor Marine Carpuat give her talk on the "Improving Machine Translation for Wikipedia" project. 

This concludes our official research for the first week! I ended up walking to some Korean BBQ -- which was fun -- with a big group (ML, SS, DS, LH, AB, SK, NL) for a late dinner. This weekend, I'm hoping to Overleaf up my notes on the papers this week and prep for a meeting with Furong early next week.

### <u>Day 6 & 7 (June 10th and 11th)</u>

First official weekend of the REU! I spent a good portion of the weekend out walking around and exercising -- I went to the UMD pool on Saturday and got a nice workout in and then played tennis with AB and AF after watching the French Open in the morning with them. Tonight (Sunday), we had a "taco night" with ML, DS, AB, SS, AF, and LH, where we made and ate tacos and nachos together. Though I got relegated to dishwashing duty in the end, it was a good time. Afterwards, I ended up throwing a football/frisbee around with LH, ML, and DS.

Research wise, this weekend, I ended up doing a bit of typing up my notes (see Notes folder for most recently updated version), but will continue to do that before meeting with our group leader Furong next Wednesday.