# Assignment 2: Protests
In recent years the United States has experienced a surge of protests, in support of Black Lives Matter, gender equity, and many other social or political issues.

In this assignment, you will work with data from [Count Love](https://countlove.org/), data that is ocassionally [cited](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html) by the _New York Times_ when reporting on US demonstrations.

Through this assignment, you will be able to answer questions about protests, including:

* What were the most attended and least attended protests in the US in the last 5 years?

* How many protests occurred in Washington state?

* How did the number of protests in 2019 compare to 2020, and why?

* Why are people protesting in the US? What are the biggest motivators?


## Learning objectives
By completing the assignment, you will develop or skills for:

- **Version control** tools for managing code (git and GitHub)
- Writing documents with **markdown** syntax
- Coding in R
- Thinking critcally about data.

# 1. Critical Analysis & Reflection: Before You Code

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out _domain familiarity_ — that is, knowledge about the topic of the dataset. Sometimes the topic is very narrow; more often it is expansive, as in the case of CountLove. We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it. To get more familiar, we are going to begin by doing some background reading.

**Note:** Please write your answers below under the heading "Your Responses and Reflections."

- First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm).  **(R1a)** Based on the information in these pieces, why did the creators start collecting the CountLove data?

- Next, we would like you to read this [New York Times piece that uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) and that describes the Black Lives Matter protests that occurred in the summer of 2020. **(R1b)** Please summarize the main point or argument of this article.

Next, we're going to reflect about who collected this data, and what's actually inside it. 

**(R1c)** Who collected and shared the CountLove data, and what do they do for a living?

**(R1d)** As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude? 

**(R1e)** How and where does CountLove get their data about the protests? 

**(R1f)** How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation? 

**(R1g)** What are two central values of Count Love? Name and briefly describe them. (See the Envisioning Cards for a defintion of "value".)

**(R1h)** Name and briefly describe one direct stakeholder and one indirect stakeholder (See the Envisioning Cards)? 

# 2. Coding in R: Parts 1-6
**Instructions**. Assignment instructions and prompts are in this file: [analysis.R](analysis.R).

**Coding and reflection prompts**. You will find two kinds of prompts in [analysis.R](analysis.R):

* *Coding prompts*, which prompt you to write R code in [analysis.R](analysis.R).
* *Reflection prompts*, which prompt you to think and write in English below, in this file (README.md).

**Formatting Your Responses and Reflections**.

* When formatting your written responses and reflections below, please *retain* all
reflection prompt IDs (e.g., R1a, R2a, etc.).
* Fill in the elipses (...) with your own words. 
* Remove expected word counts.
* To write clearly, use markdown code appropriately (e.g., **bold**, _italics_, and `code`). As appropriate, include images, links, and so forth.

**Questions?** As always, please post on Teams or ask your Instructor or Teaching Assistant.

:computer: Good coding!
   :writing_hand: Good critical thinking!
      :smile: Good-luck!

(_Updated: October 2022, Your Teaching Team_)

# 3. Critical Analysis & Reflection: After You Code

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:  
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.  
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.  
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.  
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?  

**(R1h)** How does the CountLove project embody one or more of these 4 forms of challenging power? 

**(R1i)** What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)

**(R1j)** What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)

## Your Responses and Reflections

### Critical Analysis & Reflection: Before You Code (questions above)

* **(R1a)** The creators of this data, Tommy Leung and Nathan Perkins started collecting the CountLove data because they wanted to create a factual record of ongoing demonstrations and protests across the US to make that type of data/info more accessible to citizens, politicians, and journalists. Keeping track of the number of protests can be difficult, and creating a reliable repository of that information can be incredibly helpful in fact-checking and communicating the scale of the issue to elected officials. 

* **(R1b)** The main argument of this article was to convey just how influential and impactful the Black Lives Matter movement was across the nation, through a large collection of images from protests in every single state and major city. They wanted to share the truth about the movement and how it mobilized Americans in the smallest corners of the country, despite what right-wing media may say about it only happening in bigger, liberal cities.

* **(R1c)** The creators of Countlove are Tommy Leung and Nathan Perkins, both engineers and scientists who met at MIT while working on their Masters in Technology and Policy, who were both interested in civic responsibility and public policy. They started CountLove in wake of the 2016 election and developed it through 2021.

* **(R1d)** The types of demonstrations that CountLove includes in their data are public displays of protest that are not part of a business or events put on by companies or elected officials/campaigns. The creators only wanted to count true public protests that represent a community coming together with the only motive being outrage/mobility for a cause.

* **(R1e)** CountLove gets their data from local newspapers and television sites on a daily basis. They do things called "crawling" which is a sort of process of extracting data, as well as a software stack.

* **(R1f)** CountLove makes their estimates about the number of people by interpreting certain count words as their literal estimate, such as dozen as 10, dozens as 20, and hundreds at 100. This is a potential problem and contributes to less accuracy of the data as different sources may interpret and use these count words different than others. It can also be an estimate that is too low, which is an obstruction of truth. They also mark attendances as zero when there is not mention of the a number, while still acknowledging the protest. This is even more of a loss of data.

* **(R1g)** Two central values of CountLove are transparency, with their main purpose being to provide an accurate and ongoing count of protests/demonstrations across the country. The second value is empathy, as the use of this data is meant to make more compelling cases that Americans are fighting for what they believe in and are a much more diverse, empathetic, and connected country than what the media/bad news may often portray it as.

* **(R1h)** One direct stakeholder in the CountLove data are the users of the data; this could be citizens, journalists, or politicians, just anyone who uses the CountLove data for a certain purpose or motive with the data. The indirect stakeholders would be those who were in the protests or news sites reporting on the protests with no knowledge of their presence/reporting creating the CountLove data. They may not be using the data but are indirect stakeholders of the data are being affected by it as they are the ones making those numbers happen.

### Part 3: Locations (`analysis.R`)
* **(R3a)** The number of protests in WA does not surprise me that much.
            The majority of those protests occurred in Seattle, 
            a city that is average sized, but still does not match  
            up to the scale of states who experience protests all 
            over, not just in one city. WA’s proportion of protests 
            is about 8%.
            
* **(R3b)** I do think this is an amazing feature, and one of the
            greatest parts about R functions. They make analyzing
            and summarizing data incredibly efficient.
            
* **(R3c)** The biggest data quality issue that I notice
            is the lack of context about what the values in
            the table summary mean, such as frequency.
            Frequency does not always mean counts, making
            it confusing for readers. This data would 
            make more sense displayed as a histogram.

### Critical Analysis & Reflection: After You Code (questions above)
* **(R7h)** I think that the The CountLove data embodies the forms
            of Count and Analyze the best to challenge the power
            of the hierarchy/systemic issues that lead to people
            protesting in the first place. They are taking responsibility
            and authority to collect accurate data about our country's 
            oldest right; assembly. Not only is the data they are collecting
            specific, organized, and informative, but almost self-analytic. 
            The answers are in the numbers. They show how our country can come 
            together to fight for what we believe in more often (and on a
            larger scale) than people may think, all through algorithms 
            and data science. 
            
* **(R7i)** The most interesting thing that I learned from this analysis
            was the massive variation in the purposes and motivations 
            of these protests. Many may use CountLove or see it as more useful
            for specifically the BLM Movement, like the NYT, but there is so
            much more than that. From healthcare to the environment, it is
            so cool to see the different purposes Americans use their right
            to assembly for.
            
* **(R7j)** I would love to do more visualizations with this data, such 
            as making more complex graphs like histograms and bar charts.
            I think visual references are great tools at truly showing
            the impact of data and probably part of the reason that
            CountLove's maing way to display their data was on a giant
            map of the US. 
