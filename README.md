# Database for Emotion Recognition from Speech in a Subject-Independent Setting

The dataset includes features extracted from two databases: RAVDESS and EMO-BAJKA. An important aspect of its structure is the division into three independent subsets: training, validation, and test. 
The split was performed in such a way that no features or utterances from individuals present in the training set appear in the test set. This design supports research on emotion classification in a subject-independent setting.

# Dataset Description
The dataset includes features extracted from two databases: RAVDESS and EMO-BAJKA. It contains the following files:
EMO-BAJKA_speech_features_1s_window_0.1s_overlap.mat – feature matrix for the EMO-BAJKA dataset, extracted using a 1-second analysis window with 0.1-second overlap
RAVDESS_speech_features_1s_window_0.1s_overlap.mat – feature matrix for the RAVDESS dataset, with identical segmentation parameters
Emotion Classes - EMO-BAJKA.txt – list of emotion labels used in the EMO-BAJKA dataset
Emotion Classes - RAVDESS.txt – list of emotion labels used in the RAVDESS dataset
FeatureDescription.mat – file containing descriptions of all extracted features.





