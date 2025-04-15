# Cyberbullying-Post-Role-Dataset

## Dataset Description
This dataset contains 11,977 samples of cyberbullying posts and their participant roles. 

**Cyberbullying roles data_original.CSV** 

This file includes data that has been initially coded, it is annotated with:
- `participant role`: [bullies, outsiders, assistants, defenders, and reporters]
- `Clean Text`: processed text of the posts
- `Case and its categories`: [lgj_societal case, kj_sports case, ryz_entertainment case]

**Role-emotion-analysis.xlsx** 

This is the sentiment analysis result of 11,601 posts (A small number of posts were removed in the secondary cleaning), annotated with:
- `text`: Original comment text *(linked to main dataset via comment_id)*  
- `category`: cyberbullying role [bullies, outsiders, assistants, defenders, and reporters]
- `angry`: [0,1]  
- `surprise`: [0,1]  
- `sad`: [0,1]  
- `fear`: [0,1]  
- `neutral`: [0,1]  
- `happy`: [0,1]  

The data is used for research, please contact the authors if you need to use it.

## Collection Methodology
- Source: Sina Weibo
- Collection Time：2020.8.25-2020.12.1
- Selction criteria: case must arouse considerable public concern
  - over 140 million reads
  - over 30,000 discussions
- Annotation method: Two rounds of manual coding (5 coders) + NLP for sentiment analysis
- Cleaning process： (1) remove duplicates, whitespaces, hyperlinks, unknown characters, user mentions, and HTML tags; (2) convert traditional Chinese into simplified Chinese; (3) retain emojis with matching words.

## Ethics & Privacy
- All personally identifiable information has been removed 
- Texts have been anonymized (excpet the main subjects of the case)
- The coding for roles was based on context and discourse intension, not user-level
