# Language Translation with seq2seq

A machine learning project using seq2seq, among other techniques, to create a language translator that will be able to translate between English and French. 

In this project, we'll take a small dataset that contains 227 english sentences and their french translations. The dataset contains sentences such as this one:

`English: new jersey is sometimes quiet during autumn , and it is snowy in april .`
`French: new jersey est parfois calme pendant l' automne , et il est neigeux en avril .`


(which makes no sense to me, but that is besides the point :-P )

General steps:

1. Turn words into ids

2. Make sure we designate the end of a sentence using '<EOS>'

3. Create placeholders for the input, targets, learning rate, and keep probability

4. Add '<GO>' to the beginning of each batch & remove last word id from each batch

5. Create an encoder RNN layer

6. Create training logits

7. Create inference logits

8. Build the decoding layer

9. Build the neural net

10. Set our hyperparameters

11. Build the graph

12. Train - accuracy is ~93% (could be higher if we upped the epochs and let it train for longer)

13. Preprocess our sentence to be translated

14. Translate our sentence



[Built to meet Udacity's specifications.](https://review.udacity.com/#!/rubrics/826/view)