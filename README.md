# Hearing the unheard, seeing the unseen:
Automated sign language recognition for
emergency situations


Deaf-mute people primarily communicate via manual-visual modality through sign language and hand gestures. Although these communities use sign language
to communicate among themselves, there still exists a serious communication
gap with normal people and this gap pushes the deaf-mute community towards
isolation and creates hindrance towards their personal safety. Moreover, there
are huge chances of the deaf-mute community getting underserved in the case of
emergencies due to the communication gap. To bridge this gap for such scenarios,
we propose an automated system which can recognize dynamic hand gestures
for Indian Sign Language(ISL) in emergency cases. This system would have the
capability of classifying ISL gestures into eight emergency words (namely, `ac-
cident', `call', `doctor', `help', `hot', `lose', `pain' and `thief'). As an extended
functionality, we further intend to perform real-time automated monitoring for
emergency related sign language recognition using the CCTV cameras.
For the previous solutions, the feature extraction was performed by detect-
ing only the global level features using pretrained CNN models. Moreover, the
most recent work comprised of detecting both local and global features using
computer vision algorithms and pretrained CNN models respectively. This re-
cent approach added an extra overhead by implementing multiple techniques for local feature extraction. With our proposed solution, we plan to make use
of pretrained vision transformers which implement the multi headed attention
mechanism, and therefore, there is no need to perform local and global level
feature extraction separately. Thus, our approach not only focuses on extract-
ing global features but also focuses on extracting local features without using
multiple algorithms/techniques.
We are proposing an automated sign language recognition system which can
detect emergency related sign language gestures from video footage. The key
frames extracted from the video would be passed through an encoder of a vision
transformer(ViT) to extract feature(attention) maps. These feature maps would
then be fed into a Bidirectional LSTM model for classi cation of long-range
sequences of sign language gestures into one of the eight categories of emergency
words.
