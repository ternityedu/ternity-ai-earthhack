# Ternity AI EarthHack
Official submission repo from team Ternity AI for the AI EarthHack competition

### Instructions

1. Download knowledge base of articles into local copy of repository.
   Some articles are not open access, hence the exclusion of the entire `rag_kb` folder from this public repo. The folder contains two sub-folders, one for each role ("internal monologue") that CirconBot can take on, "investor" and "scholar".
   Link: https://www.4shared.com/folder/Ja_zfK4n/rag_kb.html
   pw: repo name with parts in reverse order, no hyphens or spaces

2. Run the following to install requirements, preferably on Python 3.11.

   ``` pip install -r requirements.txt ```

3. Edit `DATA_FILENAME` and `WORDCLOUD_FILENAME` in `main.py`. `DATA_FILENAME` should point to a file with the same format as `AI EarthHack Dataset.csv`, the training dataset provided for the AI EarthHack. Optional `CLEANED_DATASET` can be specified to load a pickled cleaned dataset.

4. Run `main.py` to generate two wordclouds of the key words in both problems and solutions within the dataset. This gives the user a way to visualize the key concepts and ideas in the dataset. One could then be on the lookout for pitches that _don't_ include these most common ideas, if one were to seek innovative solutions.

   ``` python3 main.py ```

5. (Optional) You will likely notice the wordclouds dominated by a few big words. Some have already been manually excluded, but you can add more words to exclude by adding them to the `EXCLUDE` list in `utils.py`. This allows you to focus on whichever level of generality you want (e.g. one could exclude many of the most general words to get a sense of specific ideas).

### AI Philosophy
For all the claimed advancements in GenAI and LLMs these past few years, we would argue that relatively little _true_ progress has been made since the Transformer and BERT in 2017-18, upon which all major models today are built. While there have been some model improvements, the bulk of performance gains has been from simply larger models with more parameters and compute to train. As Ternity AI Founder Haihao Liu proposed in 2020 for his doctoral thesis (under "Graduate Research Fellow" at https://www.linkedin.com/in/haihaoliu/details/experience/), it will be the explicit incorporation of domain knowledge into models, deeply embedded and encoded in the model architecture itself, that will finally bring us out of this plateau.
