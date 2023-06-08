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
 - 10 AM - 12 PM: We continued to read the [Fair Diffusion Paper](https://arxiv.org/abs/2302.10893) and [another paper](https://arxiv.org/pdf/2302.00070.pdf) that addresses biases implicit in text prompts. As of now, our project focus seems to be on fairness in diffusion models and generative AI, and so I anticipate that these papers will be the glue to our project. The main goal of my paper reading today was to understand and discuss the concepts of these papers and to think about potential avenues for exploration/extension as a group. We had a productive group discussion about the concepts in the first paper and what we might explore, namely situations where prompts have implicit biases. 
 
    The first example presented in the paper is "give a photo of the face of a firefighter." To address the explicit gender bias (`men` associated to the word `firefighter`), the paper proposes using a lookup table (mapping firefighter to the gender bias) and "guidance" (consisting of an emphasis on females and a de-emphasis on males) to adjust for this bias. We are curious how this work could be extended to implicit biases: for example, the prompt "give a photo of a hospital" might yield predominately male doctors.

- 1:30 - 4:00 PM: One of group members had to leave early, so that left us with me, SS, and AF. We began reading the second paper which attempts to address biases in text prompts (using orthogonal projections to create a projection matrix that essentially acts to project out biased directions) and thought about how that might apply to the work we're interested in. We also had more casual talks about research as a whole and previous/friends' research experiences. I'm quite happy with the communication and transparency we have in the group about the process as a whole (especially with SS and AF) and so I'm hoping this will lead to a solid research group and effort this summer.

- 4:00 - 5:00 PM: We listened to Bill Gasarch (program director) give his [Muffin Problem](https://www.cs.umd.edu/users/gasarch/MUFFINS/muffins.html) talk which was quite fun/informative. I asked Bill if he would be around at Swarthmore to advertise the REU (I was thinking of getting him to give the talk as well), but he said he wouldn't be back until the next year. Bummer -- I hope when I am older I can be as energetic as Bill is.

After research, I grabbed some Q-Doba (QD) from the Union, ate, and then headed back to the dorm with ML, AB, and LH. I talked about sports with DS for quite a while, "worked", and will probably end up playing board games later as well. 

All in all, I'm happy with the direction my group is starting to work towards after just a few days of paper reading and meeting, and pretty pleased with the communication about the process/openness about my research group with regards to general social conversations and group expectations.