# SMS Spam Message Classification


## Data

Dataset available [here][dataset]

The dataset is labeled, and contains two labels of text messages: spam and ham. It is in text file format.

Dataset size: 5574 labeled messages.

Following are some examples:

|message label | message content|
|--------------|----------------|
|ham           | What you doing?how are you?| 
|ham           |Ok lar... Joking wif u oni...| 
|ham           |dun say so early hor... U c already then say...| 
|ham           |MY NO. IN LUTON 0125698789 RING ME IF UR AROUND! H*| 
|ham           | Cos i was out shopping wif darren jus now n i called him 2 ask wat present he wan lor. Then he started guessing who i was wif n he finally guessed darren lor.| 
|spam          | FreeMsg: Txt: CALL to No: 86888 & claim your reward of 3 hours talk time to use from your phone now! ubscribe6GBP/ mnth inc 3hrs 16 stop?txtStop| 
|spam          |Sunshine Quiz! Win a super Sony DVD recorder if you canname the capital of Australia? Text MQUIZ to 82277. B |
|spam          | URGENT! Your Mobile No 07808726822 was awarded a L2,000 Bonus Caller Prize on 02/09/03! This is our 2nd attempt to contact YOU! Call 0871-872-9758 BOX95QU |

## Goal
Classify the messages into spam or ham using [Support Vector Classification][sklearn-svc] 

## Method and Result
The program was developed using Google Colab notebook. I uploaded a copy of the [notebook](./svm_spam_detector.ipynb).

Best result found:

|Metric|Score (%)|
|------|-----|
|Spam Caught| 83.89 |
|Blocked Ham| 0.00 |
|Accuracy| 97.85 |
|Matthews correlation coefficient (MCC)| 90.48 |


## Discussion
Results are discussed in this [report](./SPAM_Classification.pdf).

[dataset]: https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection
[sklearn-svc]: https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html
