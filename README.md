This is a chrome extension to detect racial-based biases in article headlines as you peruse the net.

## Roadmap:

### ML-related

- [x] Grab corpus from Standford study
  - https://www.cs.cornell.edu/~cristian/Biased_language.html
  - __Note__: the actual NPOV (neutral point of view corpus) is 100GB, might 
    have to work completely off of Google Cloud to host this, and/or slim down the size for development purposes. Another option is, of course, sacrifice the hard disk size locally. 😅
- [] Collect biased article titles
- [] Determine a model to feed data
- [] Train a model to detect racial-based article titles
- [] Optimize for accuracy

### Browser related

- [] Build chrome extension application (limited to 5 newsfeeds for now)
- [] Design an `icon.png` (for browser extension icon)
- [] Design a UX to display biased based articles (jquery-related)
  - [] Textio inspired interface with different colour highlights for 
    various kinds of levels biases. ie. Assertive language, unnecessary racial 
    profiling, lack of racial profiling in commonly racially toned headlines
    bc the attacker/perpetuator is white
  - [] Cursor floatover legend for different coloured highlight markers.

### Combine the two technologies

- [] Host ML and corpus algorithm in Google Cloud
- [] Build API for extension to interact with algorithm 

### Testing
- [] Random list of 5 newslists for `manifest.json` to load 
- [] Does it flag appropriately?
- [] Does it flag inappropiately?

### Nice-to-haves:

* Recommendation UI for user to feedback into RNN
* The machine learns to suggest corrections
* Feed back into machine to improve data recognition
* Breakdown on why something is biased, simliar to [Textio](https://textio.com/tour/)
* On/off switch for users to "augment" text, or just flag

## Articles Refs (In-progress):

__Note__: Should you find any more relative links or articles on this subject, feel free to submit a PR and add for additional reading.

### Wellspring Article
This project was inspired and based off of this study:
* [Linguistic Models for Analyzing and Detecting Biased Language](https://web.stanford.edu/~jurafsky/pubs/neutrality.pdf)

### Worthwhile Citations (from Google Scholar) [_HEAD/directory tree_](https://scholar.google.ca/scholar?biw=1280&bih=632&bav=on.2,or.r_cp.&um=1&ie=UTF-8&lr&cites=888001583475750049)
* [Automatic Extraction of News Values from Headline Text](http://www.aclweb.org/anthology/E/E17/E17-4007.pdf)
* [The Impact of News Values and Linguistic Style on the Popularity of Headlines on Twitter and Facebook](http://eprints.whiterose.ac.uk/115200/)
* [Detecting and Identifying Bias-Heavy Sentences in News Articles](http://web.stanford.edu/class/cs224n/reports/2741414.pdf)
* [Identifying Political Bias in News Articles](http://www.ieee-tcdl.org/Bulletin/v12n2/papers/lazaridou.pdf)
* [Ideological Phrase Indicators for Classification of Political Discourse Framing on Twitter](https://www.cs.purdue.edu/homes/john1187/pubs/nlpcss_2017.pdf)
* [Stance and Sentiment in Tweets](http://dl.acm.org/citation.cfm?id=3003433)
  


### Other interesting articles
* [Six Harmful Patterns in Newspaper Presentations of Race](https://www.frameworksinstitute.org/assets/files/PDF_race/cognitive_media_analysis.pdf)
* [Example of Media Bias Archive](https://www.studentnewsdaily.com/archive/example-of-media-bias/)
  * [Misleading headline](https://www.studentnewsdaily.com/example-of-media-bias/misleading-headline/)
  * [Harvard Study reveals media bias](https://www.studentnewsdaily.com/example-of-media-bias/harvard-study-reveals-media-bias/)
* [Twitter Bias: We Listen When Men Talk Tech and Women Talk Diversity](https://www.recode.net/2015/9/8/11618334/twitter-bias-we-listen-when-men-talk-tech-and-women-talk-diversity)
* [Media Tenor - Creating Perception](http://us.mediatenor.com/en/chart-of-the-week/politics/1095/fox-consistently-supportive-of-republican-politicians)
* [The Impact of News Values and Linguistic Style on the Popularity of Headlines on Twitter and Facebook](http://eprints.whiterose.ac.uk/115200/)

## Datasets
* [Biased Language](https://www.cs.cornell.edu/~cristian/Biased_language.html)
* [News Aggregator Dataset - Headlines and categories of 400k news stories from 2014](https://www.kaggle.com/uciml/news-aggregator-dataset)
* [Online News Popularity Data Set](https://archive.ics.uci.edu/ml/datasets/online+news+popularity)

## Final Notes

### Namespacing

The repo's name _alpha-bias_ is a tentative name based on the common iteration 
pattern and the problem it attempts to tackle. While racially unbiasing is this project's main objective, hopefully there will be a move to expand this 
tool beyond racial bias to gender, queer, and trans related biases. This is no 
way affiliated with Google's AlphaGo or similar Alpha modelling types. 
