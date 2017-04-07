# Textual-Style-Transfer
This is an on-going project attempting to construct an analog for text to [what was so successfully done for images.](http://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf) The end goal is to build a machine learning algorithm that will transform any given English sentence into a new sentence with a similar semantic meaning but in the style of the novelist Jane Austen.

The idea - which follows the idea implemented for images - is to build two cost functions on the set of all sentences. The *style function* judges the extent to which Jane Austen might've written the sentence. The *semantic function* judges the extent to which a sentence has the same meaning as the input sentence. Given these, I plan to use stochastic gradient descent to find the sentence which minimizes (some optimal linear combination of) these functions.

I have already built the style function using a Long-Short Term Memory Recurrent Neural Network in Keras, which you can find in the .ipynb file. I am currently working on building a better semantic function. So far I have used the NLTK library's Doc2Vec with unsatisfactory results. This seems to be limiting factor for this project. If you have any suggestions about this component, or any other, please let me know.

![Under Construction](https://github.com/michaelaaroncantrell/Textual-Style-Transfer/blob/master/images/construction.png)

