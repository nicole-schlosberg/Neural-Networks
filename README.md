# Neural Networks

Neural networks are not a new method, the first artificial neural network was devised in 1943, but advances in computational power and speed have made them a much more viable strategy for solving complex problems over the last 5-10 years. Originally devised by mathmaticians and neuroscientists to illustrate the fundamental principles of how brains might work they lost favor in the second half of the 20th century only to surge in popularity in the 20-teens as software engineers used them to resolve mathmatically intractable problems. The application of neural networks to learning problems has been ongoing for 20 years, often to predict student behvior or to parse unstructured data such as student writing samples and provide natural sounding feedback through AI avatars.

* My neural network to predict student attentional state from webcam images. 

## Goals

* Be able to explain the utility of artificial neural networks
* Be able to explain the backpropagation algorithm
* Be able to build a basic neural network to solve a prediction problem

## Reflection on my neural network

*How accurate is your neural net? How can you tell?* When you run the metrics using the confusion matrix and statistics on the neural net, the model's accuracy is at 98%. The sensitivity (true positive rate) is at 1.00, indicating that the rate correct classification of a students paying attention is 100%, and the specificity (true negative rate) is at 0.9683, suggesting that the rate correct classification of a students not paying attention is 96.83%. This means that the model is good at accounting for true positives and true negatives.

*How would you explain your model to the students whose behavior you are predicting?* I would explain that each on of the input data (eyes, face.forward, chin.up, squint, hunch, mouth1, mouth2, mouth3) tell us whether they are paying attention. So if they they are facing forward (1) then that shows one aspect of paying attention. If their chin is up (1) then we have another factor that shows they are paying attention. If there are enough of these factors (inputs) that represent paying attention then the model will meet its threshold. In other words, it will pass an inspection that meets the qualifications for paying attention. The prediction metrics shows how well this model is at predicting those that are paying attention are actually paying attention and those that are not paying attention are in fact not paying attention.

*This is a very simple example of a neural network. Real facial recognition is very complex though. Would a neural network be a good solution for predicting real facial movements? Why, why not?* Using a neural network for real facial recognition would be very flawed. Human facial expression is very diverse. We might all have the same facial emotions, but how we actually present them or hold our selves can be very different both culturally and simply genentics. These vast array of facial nuances are likely not going to be able to be accounted by a simple neural network model, thus many of such nuances will get lost and not recognized. Thus the prediction would be wildly off.

## Codebook

In the attached data sets attention1.csv and attention2.csv, you will find data that describe features associated with webcam images of 100 students' faces as they participate in an online discussion. The variables are:

eyes - student has their eyes open (1 = yes, 0 = no)
face.forward - student is facing the camera (1 = yes, 0 = no)
chin.up - student's chin is raised above 45 degrees (1 = yes, 0 = no)
squint - eyes are squinting
hunch - shoulders are hunched over
mouth1 - mouth is smiling
mouth2 - mouth is frowning
mouth3 - mouth is open
attention - whether the student was paying attention when asked (1 = yes, 0 = no)

## Utilized the following resources

[![Introduction to Neural Networks](https://img.youtube.com/vi/x54ULLJSzBM/0.jpg)](https://youtu.be/x54ULLJSzBM)

[Video Slide Deck](https://github.com/la-process-and-theory/neural-networks/blob/master/HUDK4051-neural-nets.pdf)

[Sanderson, G. (2017). But what *is* a Neural Network? 3Blue1Brown. ](https://www.youtube.com/watch?v=aircAruvnKk)

[Bling, S. (2017). MariFlow - Self-Driving Mario Kart with Recurrent Neural Network](https://www.youtube.com/watch?v=Ipi40cb_RsI)

Nielsen, M. (2015). Neural Networks & Deep Learning. Determination Press:San Francisco, CA  
  [Chapter 1](http://neuralnetworksanddeeplearning.com/chap1.html)  
  [Charpter 2](http://neuralnetworksanddeeplearning.com/chap2.html)  

[McKlin, T., Harmon, S. W., Evans, W., & Jones, M. G. (2001). Cognitive presence in Web-based learning: A content analysis of students' online discussions.](https://files.eric.ed.gov/fulltext/ED470101.pdf)  

For more detail:  
[Stergiou, C. & Siganos, D. (2000). Neural Networks.](http://www.doc.ic.ac.uk/~nd/surprise_96/journal/vol4/cs11/report.html)

[Hartnett, K. (2019). Foundations Built for a General Theory of Neural Networks](https://www.quantamagazine.org/foundations-built-for-a-general-theory-of-neural-networks-20190131/)

[Lewis-Kraus, G. (2016). The Great AI Awakening. The New York Times: New York, NY](https://www.nytimes.com/2016/12/14/magazine/the-great-ai-awakening.html)

[Roberts, E. (2000). History in Neural Networks. Stanford University: Palo Alto, CA](https://cs.stanford.edu/people/eroberts/courses/soco/projects/neural-networks/History/history1.html)
