# Dataset Description 
Our dataset consists of Haikus. Haiku is a type of short form poetry originally from Japan. Traditional Japanese haiku consist of three phrases that contain a kireji, or "cutting word", in a 5, 7, 5 pattern, and a kigo, or seasonal reference. 
We have collected Haikus from 4 different sources - which majorly scrape these poems from web. Although original Japanese Haiku followed a theme around nature - the Haiku's collected have varied themes.

## Details 
The dataset has over 140k Haikus from different sources namely Tempes Libres, Haikuzao corpus, PoetRNN corpus 

## DataType
Haiku is a 3 line poem - the first 3 columns refer to the three sentences of the haiku, we also store the source of the dataset. Our next feature is count of syllables in each line.

The dataset is a comma separated value indexed as -
0,1,2,source,0_syllables,1_syllables,2_syllables

We have a total of 143,147 haikus for training purposes. Since our aim here is to train a generative model we plan to use all of our poems for training the model, we use the 80-20 split for Training and Developement set. The poems generated by our model will then be analysed using Evaluation metric to access the quality of model. 

### Data Row Counts 
In this dataset we have 6 unique sources - ['twaiku', 'img2poems', 'gutenberg', 'haikuzao', 'sballas', 'tempslibres'].
#### Train set - train.csv has 114,509 haikus
Out of the total 74695 follow the 5-7-5 structure.

#### Development set - dev.csv has 28628 haikus
Out of the total 18695 follow the 5-7-5 structure.