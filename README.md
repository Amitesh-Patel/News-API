# News-API

Web App - `https://newsify-git-main-ad1tyakumar.vercel.app/`

API url - `AmiteshPatel.pythonanywhere.com` -- It will display Hello World
 
Its has endpoint  `/search/{text query}`  - enter your search in that text query

Ex -  `https://amiteshpatel.pythonanywhere.com/predict_api/IPL`

Second End point for to get news by categories . 
Its has following categories --  [WORLD, NATION, BUSINESS, TECHNOLOGY, ENTERTAINMENT, SPORTS, SCIENCE, HEALTH]
Just enter the index of category you want suppose you want news on category Technology - then enter 3 (Remember it follows python indexing)

`/topic_news/{number}` -- to get news by category

Ex - `https://amiteshpatel.pythonanywhere.com/topic_news/4`
The content of JSON are summary , article , sentiment etc

Json has following fields .

`
{

        "Article": "The debate over strike rate or progression of the metric over the course of a knock or an innings has been among the hotly debated topics amid the thrillers in IPL 2023. Most recently, former RCB skipper Virat Kohli was savaged on air by former New Zealand cricketer Simon Doull, who lashed out at the star batter for prioritising “personal milestone\". But Kohli has now responded to the strike rate criticism with a fitting reply. Virat Kohli; Simon Doull\n\nIn the IPL 2023 game between RCB and Lucknow Super Giants at the Chinnaswamy earlier this week, Kohli had started off on a great note. 34 of his 42 runs which came in the powerplay were ",
       
       "Headline": "'There are many people who...': Kohli's apt reply to Doull's 'milestone' jibe - Hindustan Times",
       
       "Keywords": ⊕[ ... ],
       
       "Publish date": "Sat, 15 Apr 2023 02:02:01 GMT",
        
       "Sentiment": "Positive",
       
       "TextClassification": "Politics",
        
        "Url": "https://news.google.com/rss/articles/CBMiqAFodHRwcz",
        
        "id": 2,
        
        "images": "https://www.hindustantimes.com/ht-img/img/2023/04/14/1600x900/doull_kohli_1681144795076_1681485360309_1681485360309.jpg",
        
        "summary": "The debate over strike rate or progression of the metric over the course of a knock or an innings has been among the hotly debated topics amid the thrillers in IPL 2023.."
    
    },
`

Most important fields are sentiments , Text classification because on both of these i used Bert model to classify sentneces . 
