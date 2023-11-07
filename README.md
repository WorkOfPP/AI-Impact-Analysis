# Background
In March of 2023, [Goldman Sachs published a report](https://www.aei.org/articles/why-goldman-sachs-thinks-generative-ai-could-have-a-huge-impact-on-economic-growth-and-productivity/), indicating that ~25% of the tasks in US and Europe can be automated using AI.  However, as you can see in [this visualization](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F20fefbbb-4dbb-41fe-bd6f-5f7e856abd52_1169x600.jpeg), not all industries will be affected equally.  According to the report, certain jobs, like office tasks, legal, architecture and social sciences have a potential for 30%+ automation, while positions like construction, installation and building maintenance are going to be largely unaffected.

You can also see supporting evidence in the [Facebook Research paper](https://ai.meta.com/blog/robots-learning-video-simulation-artificial-visual-cortex-vc-1/?utm_source=linkedin&utm_medium=organic_social&utm_campaign=research&utm_content=video), which highlights Moravec’s paradox, the thesis that the hardest problems in AI involve sensorimotor skills, not abstract thought or reasoning, which coincide with Goldman Sachs predictions.

While both of these papers are very impressive, they also heavily influenced by the recent advances in Large Language Models (LLMs).  For this final project I have prepared a collection of ~200K news articles (about 900 MB) articles on our favorite topics: Data Science, Machine Learning and Artificial Intelligence, and I want you to identify what industries and job lines are going to be most impacted by the AI over the next several years, based on the information you can disseminate from this text corpus.

# Objective
The goal of this project is:
- to identify what types of tasks and jobs are most likely to see the biggest impact from AI by extracting meaningful insights from unstructured text.
- to provide actionable recommendations on what can be done with AI to automate the jobs and / or improve employee productivity.
- to pay attention to the introduction of novel technologies and algorithms, such as AI for image generation and Conversational AI, as they represent the entire paradigm shift in adoption of AI technologies and data science in general.

# Data
Note: this is live data, so the layout and record counts in your dataframe will vary from the counts in the attached notebook
Download data from https://storage.googleapis.com/msca-bdp-data-open/news_final_project/news_final_project.parquet

# Steps
1. Clean-up the noise, by eliminating newlines, tabs, remnants of web crawls, and other irrelevant text
2. Discard irrelevant articles
3. Detect major topics
4. Identify top reasons for successful data science / AI initiatives (sentiment analysis) - these can be related to technology maturity, people, data availability, etc.
   - Suggest why certain types of applications succeed vs other fail
   - Plot a timeline to illustrate how the sentiment is changing over time
5. Identify new technologies and AI solutions that might be affecting the landscape of data science applications
   - Plot a timeline to illustrate the introduction of some of these technologies
6. Demonstrate what companies, academic institutions and government entities can do to accelerate the development of these transformative capabilities
7. Leverage appropriate NLP techniques to identify organizations, people and locations, then apply targeted sentiment
    - What types of companies (based on the lines of business) should invest in data science initiatives today or near future (success stories)? Create appropriate visualization to summarize your recommendations (i.e. word cloud chart or bubble chart)
    - What types of applications cannot currently be transformed by AI, based on today's state of technology (failures)? Create appropriate visualization to summarize your recommendations (i.e. word cloud chart or bubble chart)
 

### Additional guidance:
1. Clean-up or sample data if you need to shorten processing times or reduce memory usage
2. Default sentiment will likely be wrong from any software package and will require some tweaking
   - Keyword / dictionary approach
   - Data annotation and development of custom classifier
   - Building custom model on open-source data (i.e. Yelp)
   - Fine-tuning Transformer Pipeline
3. Topic detection : You are encouraged to explore a combination several techniques to identify key topics-
   - Topic modeling (i.e. LDA using gensim or ktrain) or using BERTopic
   - Classification (hand-label several topics on a sample and then train classifier)
   - Clustering (cluster topics around pre-selected keywords or word vectors)
   - Zero-shot (NLI) modeling
