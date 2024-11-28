# Unvarious-Pose
Unsupervised domain adaptation in human detection for various human pose

In human detection algorithms, some recurrent issues
are still challenging. Indeed, in a real application we have
a lack of various human poses in our data. For example,
in video surveillance it could be a significant issue to for-
get detecting a human in uncommon pose. We propose a
compensation to these less frequent cases. We introduce
a detection in rotated view to compensate limited various
poses in our dataset. Instead of introducing a generative
enhancement for every human body pose, which could be
exhausting. Indeed, data annotation has become a difficulty
for many applications. Moreover, a simple data augmen-
tation is not efficient to generalize our training. We need
a strategy to learn this new poses. So, we will introduce a
process to compute pseudo labels in a sequence of rotated
views. It avoids to use a clustering algorithm like dbscan[3]
or K-means to compute a pseudo label. A summary of the-
oretical results is described in a first section to illustrate
our baseline. First of all, we will illustrate how we process
pseudo label on various views by two mechanisms which
have been called relaxation and scanning. We introduce a
sequence of rotations of original view, to process a detec-
tion in a compensated view. In second step, we will learn
this distortion created by the various views and construct
an approach to distill original knowledge to a more gener-
alized training.
The main improvement of this approach is to propose an
alternative solution at dbscan[3] approach which is popu-
lar, but which is difficult to use in real applications. We ob-
tain a significant result by improving accuracy in especially
various pose datasets.
