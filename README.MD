Story Book Generator:

Use GPT API and Leonardo.ai API to generate story books with images.

Both Automatic mode, and step-by-step mode implemented:

Automatic Mode: 
will build you a book in no time, but it will be GPT's choices guiding the story. 
command:

python.exe StoryBookGenerator.py


Step-by-Step Mode:
will generate content, display content (not pictures yet) and allow the user to decide if the 
content generated is acceptable, if not, the script will run again and again wait for approval. 
when the user approves content, the script moves on to the next chapter/title/image prompt. 

command:

python.exe StoryBookGenerator.py step-by-step


Things to come: 

The code for saving each part of the story as it's generated is in the script, but i have not yet
implemented it. Feel free to mess with it, I'll clean it up in the next revision.  This will help 
for anytime the script crashes midway through. At the beginning of the script an excell file will
be checked for the completion status of the last story, if it's not been completed, the user will 
be prompted if they would like to continue the incomplete story or start new.

dependencies: 
openai API access as well as Leonardo.ai access. If you scour the code and comment out the calls to
image generation, you should be able to easily configure the script to only produce textual content, 
but to get the pictures, sign up for leonardo.ai's 12 tier, you get more than enough generations per
month to pump out all sorts of cool stories w/ images. 

pip install openai openpyxl

import openai
import openpyxl
