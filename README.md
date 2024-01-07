# Ternity AI EarthHack
Official submission repo from team Ternity AI for the AI EarthHack competition

1. run the following to install requirements,preferably on python 3.11

   ``` pip install -r requirements.txt ```

2. run huggingface_training.py to see partial results on loading the dataset

   ``` python3 huggingface_training.py ```

#### General guideline on coorporating in a repo
The main branch is protected all changes made it to the
main branch should go over a pull requests first, where members
will review your code before committing to the repo.

#### Steps to made your own change
1. check out the latest main branch:
   ``` 
   git checkout main
   git pull main
   ```
2. create a new branch from the latest version
of main, with a meaningful name. For example

``` git branch your-branch-name-here```

And checkout that branch:

``` git checkout your-branch-name-here ```

3. Your changes should be commit to your branch only.
while you have checkout your branch, run the following to make a commit.

``` git commit -m your-commit-name ```

4. After you have tested and finished your functionalities,
submit a pull requests on github to merge your branch to main.

