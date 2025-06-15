# Computer-Vision-Lab
# [Computer components AI Training]

## Project Description
For my project, I decided to use Google's Teachable Machine to classify common objects found on my desk. The objects I used were a stand-alone microphone, an energy drink, and a wireless mouse.

## Classes Identified
List the objects your model was trained to identify:
* Class 1 (Computer Mouse)
* Class 2 (Energy Drinks)
* Class 3 (MicroPhone)


## Discussion & Reflection

1.  **Model Performance & Iteration:**
    * How accurate was your first trained model? The first model that I trained almost always gave me a MicroPhone for every single Class that I showed it.
      I believed this was because the microphone class had the most angles and the most pictures.
      
    * What steps did you take to iterate and improve its performance? First off I had roughly 60-70 photos in the 3 classes but the microphone class had the most images and variation of images.
      So I first added around 500-700 more images to each section using my webcam. I noticed a slight improvement but not good enough of an improvement for me.
      I then decided to change the batch size values by one step each time until I reached 256 batch size.
      
    * How did these changes affect the model's accuracy and confidence scores? The increase in images gave me a slight performance boost but not nearly noticeable enough.
      The main change I saw was when I increased the batch size, in which almost every object I showed, it would be correct or close enough to correctness for me to allow it to pass.(which is about 80-90%)

2.  **Challenges & Observations:**
    * Which objects were the easiest for your model to learn and distinguish? Why do you think that was? My model usually has the easiest time recognizing the microphone with 100% accuracy.
      I think it is because of the unique shape my stand-alone microphone is, it can be easily decerned from the other objects.
      
    * Which objects were the most challenging? What made them difficult (e.g., similar shapes, variable appearances)? My computer mouse is the most challenging object simply for the fact it is very small when put up against the other objects.
      The mouse is also the same color as the microphone so the webcam has a hard time discerning the appearance of my mouse and my microphone.
      
    * What happened when you showed the model an object it wasn't trained on? How did the confidence scores behave, and why is this significant? Because my model is only trained on 3 objects, it is only looking for those 3 objects.
      It doesn't look like it has the ability to tell you that your object is 100% not there, for example, the energy drink I used has a multitude of colors, so if I show it something colorful it usually tells me it is an energy drink even though it could just be a shirt or a card.
      This shows that my model is either lacking variety or is not made to tell you if something is not 100% there.

3.  **Bias in AI:**
    * If you only trained your "mug" class with images of *your specific mug* (and didn't vary color, shape, etc.), how well do you think it would recognize other students' significantly different mugs? How does this illustrate the concept of bias being introduced through training data?
      I think the AI would have a hard time figuring out different mugs because it is only trained on one concept of a mug, but I feel as if the mugs were the same shape the AI would be able to tell even if by a little bit.
      Training AI in a variety is very important in the fact it needs variety to be able to tell you that a mug is not a microphone, etc.
      
    * Imagine all your training images were taken in very bright, direct lighting. What might happen if you tried to use the model in a dimly lit room or with strong shadows? How does this relate to the robustness and potential biases of AI models?
      I think the lighting can make a big difference because lighting affects the colors that are perceived and can even affect how we see shapes. AI bias is very real, for an AI to not be biased we would have to expose it to every variance possible, more variances than we have ever seen because AI cannot think for itself(yet). Unless we specifically code it to say, no that is not the right object or something of that nature.

4.  **Model Limitations & Usefulness:**
    * What are some key limitations of the model you created? The biggest limitations I can see are the lack of variety and the lack of the model to say no, that is not your object.
      
    * Why is it useful to be able to download your trained model files (like `model.json`, and `weights.bin`) and share them (e.g., via GitHub)? What does this enable? This enables an open-source project that other models can learn from without having to buy rights.
      It enables a wider variety of models of all differences and even culturally different objects, like a soda can in America versus Australia.

5.  **Real-World Applications & Ethics:**
    * Brainstorm 2-3 real-world applications where a similar image classification model could be useful. One example that could be used is the use of AI to help solve crimes/murders, especially for serial killers. AI can discern small effects that we may never see, as well as locate patterns we may never notice or see as well. Secondly, I think AI could be an amazing thing for healthcare, training AI on every disease that we have, training it on every solution we have tried to cure uncurable diseases. Then use this AI to show possible solutions we may not have found yet to cure uncurable diseases etc.
    * Briefly discuss one ethical consideration that developers should keep in mind when building and deploying image recognition AI in the real world (e.g., related to fairness, privacy, and misuse).
      In my opinion, I think AI is already very under-regulated even with image generation. With the wrong person using AI, it could be used to disrupt nations, people, etc. I think the main concern of image recognition is the ability to use it for bad things.

## (Optional) Screenshot
* 
