# sentiment_analysis

  Scratch approach:

  Aim of the model is to find whether a tweet referred as a postive sentiment or negative sentiment using Navie Bayes
  The naive bayes classfier is one of the simple probabilistic classifier used for processing text. we implemeted two methodds for naive bayes from scract

1.sentiment_analysis (slightly modified approach)
2.naive_bayes a standard approach
   
# 1.sentiment analysis(slightly modified approach
   pre-Prcoessing
    we have done pre processing only for the trianing data set 
    we have removed numbers from the data set, extra special characters.  we also trimmed exrtra white spaces. since it is not any known languages we cannot able reduce the stop word. we also tried clipping but ti deos decrease the accuracy so we avoided.
    
   Fitting the model
   i will find the total number of uniques tokens in the whole coropus 
   we first segeregate postive tweets and negative tweets, and then i will find the tolal number of words in the positive corpus and negative corpus. i will throw all the psotive words in one bag and negative words in bad along with their frequency.
   
   accuracy on the test_set: 0.5991
 
  To predict
    i will loop through all the words in the sentence and i will find two score for every word and multiply all the indicidual probability
    A the end of the predict fucntion i will be left with two socre for a single tweet.
    each tweet will have probability of sentence to be positive and porbability of sentence to be nagative . i will find the maximum of two and will predict.
    
# 2.Navie bayes standard approach
   logprior = np.log(d_pos) - np.log(d_neg)
   Both are almost the ssame the only differece is , here at the end i will predict if my predicted score is greate than logprior value i will conclude it as psotive or else negative,  
   In the standard approach we used log probabilities to avoid underflow values.
   
   accuracy on the test_set: 0.5253
   
   
