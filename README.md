# DNA-Sequencing-using-Machine-Learning-and-Deep-Learning-Algorithms

#1. OBJECTIVE
    • To obtain the better prediction accuracy out of the prediction model
    • To identify insights and get the most accurate values for decision trees, random forest, 
      Naïve Bayes algorithms, CNN, and Transform Learning.
    • Comparing the results of the ML algorithms with the result of DL algorithms.
    • Identify the better performer out of 5 distinct algorithms.
    
#2. AIM OF THE PROPOSED WORK
      The aim of the proposed system is to implement a better prediction model for DNA research
      and get the most accurate results out of it. The machine learning models which are being 
      considered are the most used and most reputed. We can expect a prediction accuracy of the 
      higher range and the neural networks in deep learning are also being used which are also the 
      better performer in different medical domains. 
      
#3. TECHNICAL SPECIFICATIONS:
      Hardware Requirements 
        • Processor: At least 1GHz. 
        • Ethernet connection (LAN) or wireless adapter (WiFi)
        • Hard disk: 32GB or higher
        • Memory (RAM): 1GB or more
      Software Requirements
        • Python 
        • Biopython Library 
        • Sklearn 
        • Numpy 
        • Pandas 
        • Matplotlib
 #4. PROJECT DEMONSTRATION
Our project is basically understanding how we can do DNA sequencing using ML, DL techniques, and algorithms. we know that DNA in our human beings consists of a sequence type ATGC or a different kind of sequence.  Here we just came across a data set in Kaggle and from that, we've basically taken up this particular project what we do is that by using DNA sequencing we will apply a classification algorithm that will be able to classify these particular sequences in human beings like to what kind of gene class the particular sequence belongs to.

We have imported a few libraries like NumPy, pandas, and matplotlib. The data is called human_data.txt, this data set we have downloaded from Kaggle. Now after running this data set, we got the human DNA sequence and their class. Basically, now we have sequence and class. Now when we read this particular dataset, based on the sequence it should be able to predict to what class the sequence belongs to. Now this sequence may be the gene sequence or a DNA sequence of a particular human being and they are basically classified into various classes. And apart from this particular data set we also have some data set for chimpanzee data and dog data which we got it from Kaggle itself and these data sets will also be having the same thing which is called a sequence and a class.

 ![image](https://user-images.githubusercontent.com/99421940/204093088-31a0a484-0f8c-4331-bf10-54c43f4a8f18.png)


                                                Fig 7.1: Gene Family

This is basically a gene family, if a particular sequence belongs to class 0 then it means that it belongs to the g protein-coupled receptors gene family, this number basically shows that class label 0 is present on 531 and so on, we just retrieved it and just saw what all this class is, and this is about gene family. 

We have used k-mer counting. When we are working with DNA sequencing or transcription, we basically convert this DNA sequences as languages, and in order to convert those into languages we basically use this particular technique k-mer counting. Here we have used words of length six which is also called as hexamers. Finally, this sequence is broken down into 4 hexamer words. In the same way our sequence will be converted into a vector by using NLP. 

Next, this particular data set will be converted into 6 sets of words, and each word of length 6. We have done this because then only we can apply count of words or bag of words for this particular data. We have done chimpanzee data and dog data. Next, we need to convert the list of k-mers for each gene into string sentences. So now we need to combine all the sequences together because once we combine them it becomes very easy for us to convert into a bag of words. Till here the same steps will be followed to chimpanzee and dog data. We will do this later. Next what we will do is that we try to convert the strings by applying bag of words by using count vectorizer. Sir we do this because we have our independent feature in the form of strings, and in NLP we cannot use data key strings directly to our model, so for this we convert the strings into bag of words using count vectorizer. Now what we do is that we check whether my data set is balanced or not, so for that I'm just finding and trying to see my human data value counts. 

 
Fig 7.2: Class Balance of Human
 
Fig 7.3: Class Balance of Chimpanzee and Dog

Now you can see over here it is very precisely all the classes are approximately balanced. Some of the datasets are low but other classes are approximately balanced so we can basically use this directly and we don't have to handle if we have the problem of the imbalanced dataset. If there is an imbalanced dataset problem then you can do oversampling. now we are doing the Train test split and I'm taking 20% as my test size. Next, we applied all our classification algorithms to our three datasets to check the accuracy. These classification algorithms are estimated using different classification metrics. All these mentioned metrics are estimated from the confusion matrix. The model performs well on human data. It also does on Chimpanzee. This is not surprising as we already know that man and chimpanzees are genetically related. But the model when used for dog data did not show good results as both man and dog are not much related to each other.

