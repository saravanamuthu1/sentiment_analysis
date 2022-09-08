# sentiment_analysis

  Scratch approach:

  Aim of the model is to find whether a tweet referred as a postive sentiment or negative sentiment using Navie Bayes
  The naive bayes classfier is one of the simple probabilistic classifier used for processing text.
   
   pre-Prcoessing
    we have done pre processing only for the trianing data set 
    we have removed numbers from the data set, extra special characters.  we also trimmed exrtra white spaces. since it is not any known languages we cannot able reduce the stop word. we also tried clipping but ti deos decrease the accuracy so we avoided.
    
   Fitting the model
   i will find the total number of uniques tokens in the whole coropus 
   we first segeregate psotive tweets and negative tweets, and then i will find the tolal number of words in the positive corpus and negative corpus.
