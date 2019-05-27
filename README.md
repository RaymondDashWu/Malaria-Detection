Initially did this as a warmup exercise to get back into the rhythm of deep learning. While it did turn out to be great practice it was also a gentle reminder datasets aren't perfect. 

Dataset from here:
https://www.kaggle.com/iarunava/cell-images-for-detecting-malaria

# Conclusions (for now)
- Time could have been saved if I had questioned the results more after my ResNet34 fine tuning. The ResNet50 took a day and a half after and I didn't really look at them too carefully. Sort of just ignored it because I wanted ResNet50 tuning practice. While there was slight improvement, my results could be summed up as the follow: training a 97% accurate model took 3-4 hours while adding an extra .5% accuracy took a day and a half.
- It seems that some of these images are indeed mislabeled. The most blatantly obvious ones would be the ones labeled parasitized when they are uninfected.
- The malaria infected/parasitized images in the plot_top_losses function are inconclusive. After asking several subject matter experts on Reddit there was a general hesitance to qualify an answer in either direction. Higher resolution images would be needed to draw a conclusion.
- Other more diagnostic and higher quality images were linked in the Reddit thread below. A future to-do could be to train addendums featuring said images with a slightly higher learning rate

Sources (Thanks Reddit!)
- https://www.reddit.com/r/pathology/comments/bt1dxn/im_a_data_science_student_and_i_made_a_classifier/
- https://www.reddit.com/r/medlabprofessionals/comments/bt30l2/im_a_data_science_student_and_i_made_a_classifier/