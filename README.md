# llm-archives

### Instructions

Click the "Use this template" button for this repository and choose "Create a new repository". You can give it the same name (llm-archives).

Once it's ready, go to [Groq](https://console.groq.com/keys) and follow the directions to get an API key. You'll need to login (or create an account if you don't have one).

Copy the API key value and then click on the Settings of your GitHub repository and click on "Secrets and variables" on the left side, then choose "Codespaces"

Click the green "New Repository Secret" button and paste your API Key into the "Secret" box, then put GROQ_API_KEY in the Name box above it. Click "Add Secret" and click on the name of the repository to return to the main page.

From there, click the green "Code" button and create a new Codespace in the Codespaces tab.

In the Terminal type the following: pip install requests groq and hit enter.

Then type: python get_stories.py

You should see a file called cns_maryland_posts.json appear. Let's look at it. It contains some details of the past 10 CNS stories.

Back in the Terminal, type: python entity_extraction.py and watch the output.

### Evaluation for JOUR389W

I chose the following article from IGN: 
https://www.ign.com/articles/returnal-anniversary-housemarque-announces-graphic-novel-and-artbook

I was pretty impressed with Groq's results. It returned every name and organization in the article. It did make some interesting organizational choices, however. I chose this article since it includes fictional people and places as well. It logged "Atropos" correctly as a place in a video game's universe, but it also logged Amazon the retailer as a place, which I would consider more an organization. Interesting it named the fictional planet but not the fictional protagonist Selene Vassos. 

I believe IGN could do a lot with a process like this. I've mentioned in other assignments how IGN could catalog their tech reviews so that readers could basically shop on IGN by looking at their different ratings of tech based on categories. A process like this could extrapolate categories of technology from a wide variety of articles which could then be implemented in an external format. 

Also, we've discussed in class about how a system like this could be used to help guide an organization's sourcing. IGN could use this to not only create a organizationally-wide pool of sources but also to sift through their sources and those named in articles to see trends of diversity or overuse. 
