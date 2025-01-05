Q) why I am not using the the metrics like F1, Recall, etc. in the training loop like in the exercise 8 (we did accuracy and loss)

A) It is less common to calculate metrics like F1 score, IoU, recall, or precision during every training iteration because these metrics usually require evaluating the model on the validation set, which can be computationally expensive. However, it is not uncommon to compute these metrics periodically during training (e.g., at the end of each epoch) to monitor the model's performance and detect overfitting or underfitting.

Common Practices:
During Training Phase:

Metrics like training loss and accuracy are often calculated during each iteration or mini-batch because they are easy to compute and directly tied to the optimization process.
Computing more complex metrics like F1, IoU, recall, or precision on the training set might not provide much insight since the model is being optimized on this data. The training set metrics tend to be inflated and do not reflect the model's generalization ability.
Validation Phase (After Each Epoch):

Computing metrics like F1 score, IoU, recall, and precision on the validation set is a common practice. These metrics help evaluate how well the model is generalizing without needing to test on the actual test set during training.
It’s typical to track these metrics after each epoch (once the model has seen the entire training set) rather than at every iteration, as validation involves running the model inference on a separate dataset.
When to Use Complex Metrics During Training:

For segmentation tasks (like IoU) or classification tasks (like F1 score), these metrics can be tracked on the validation set during training if they are critical to your project's goals.
If you are using an early stopping strategy, monitoring these metrics can help determine when to halt training to prevent overfitting.
When to Avoid Computing Metrics:
Real-Time Constraints: Calculating these metrics during every iteration may slow down training, especially for large datasets or models.
Non-Binary Metrics: For multi-class or multi-label problems, metrics like F1 or IoU often require specific averaging (e.g., macro, micro) and careful handling, making them less straightforward to compute frequently.
Recommendations:
Training Set: Track only loss and, optionally, accuracy during iterations/epochs.
Validation Set: Compute F1, IoU, recall, and precision after each epoch to analyze the model's generalization ability.
Final Evaluation: Use the test set only after training is complete for the final evaluation of these metrics.

1. I have to write regardig the evalution dataset (manual labeling)
2. postive and negative examples of the images, why I excluded some of them, how many excluded
3. image examples
4. the used models and sources of the models (scientifc papers)
5. the results of the dusseldorf and soest datsets


6. for the reults two points: 1. the number of the founded images (plus or minus) (step 1)
                            2. improve the results of the founded area with the known knoledge we have bounding boxes with regularity of the windows (height and width) 