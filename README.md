This is a chrome extension to detect racial-based biases in article headlines as you peruse the net.

## Roadmap:

### ML-related

- [] Grab corpus from Standford study
- [] Collect biased article titles
- [] Determine a model to feed data
- [] Train a model to detect racial-based article titles
- [] Optimize for accuracy

### Browser related

- [] Build chrome extension application (limited to 5 newsfeeds for now)
- [] Design an `icon.png` (for browser extension icon)
- [] Design a UX to display biased based articles (jquery-related)

### Combine the two technologies

- [] Host ML and corpus algorithm in Google Cloud
- [] Build API for extension to interact with algorithm 

### Testing
- [] Random list of 5 newslists for manifest.json to load 
- [] Does it flag appropriately?
- [] Does it flag inappropiately?

### Nice-to-haves:

* Recommendation UI for user to feedback into RNN
* The machine learns to suggest corrections
* Feed back into machine to improve data recognition
* On/off switch for users to "augment" text, or just flag

Articles Refs (In-progress):

__Note__: Should you find any more relative links or articles on this subject, feel free to submit a PR and add for additional reading.

https://web.stanford.edu/~jurafsky/pubs/neutrality.pdf
https://www.studentnewsdaily.com/example-of-media-bias/misleading-headline/
http://us.mediatenor.com/en/chart-of-the-week/politics/1095/fox-consistently-supportive-of-republican-politicians
https://www.studentnewsdaily.com/example-of-media-bias/harvard-study-reveals-media-bias/
http://eprints.whiterose.ac.uk/115200/
http://web.stanford.edu/class/cs224n/reports/2741414.pdf
http://dl.acm.org/citation.cfm?id=3003433
https://arxiv.org
