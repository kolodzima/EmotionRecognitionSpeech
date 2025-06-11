# Database for Emotion Recognition from Speech in a Subject-Independent Setting

The dataset includes features extracted from two databases: RAVDESS and EMO-BAJKA. An important aspect of its structure is the division into three independent subsets: training, validation, and test. 
The split was performed in such a way that no features or utterances from individuals present in the training set appear in the test set. This design supports research on emotion classification in a subject-independent setting.

# Dataset Description
The dataset includes features extracted from two databases: RAVDESS and EMO-BAJKA. It contains the following files:

- EMO-BAJKA_speech_features_1s_window_0.1s_overlap.mat – feature matrix for the EMO-BAJKA dataset, extracted using a 1-second analysis window with 0.1-second overlap

- RAVDESS_speech_features_1s_window_0.1s_overlap.mat – feature matrix for the RAVDESS dataset, with identical segmentation parameters

- Emotion Classes - EMO-BAJKA.txt – list of emotion labels used in the EMO-BAJKA dataset

- Emotion Classes - RAVDESS.txt – list of emotion labels used in the RAVDESS dataset

- FeatureDescription.mat – file containing descriptions of all extracted features.

- #  Structure and Partitioning

The dataset is divided into three independent subsets:

- **Training set** (`cechy_Train_all`)
- **Validation set** (`cechy_Validation_all`)
- **Test set** (`cechy_Test_all`)

No utterances or speakers from the training set are included in the test set, enabling a **subject-independent evaluation**.

### Variables in `.mat` Files:

| Variable Name           | Size       | Description                                                                 |
|------------------------|------------|-----------------------------------------------------------------------------|
| `cechy_Train_all`      | 2376 × 97  | Training data: 2376 samples, 96 features + 1 label column                   |
| `cechy_Validation_all` | 336 × 97   | Validation data: 336 samples, 96 features + 1 label column                  |
| `cechy_Test_all`       | 687 × 97   | Test data: 687 samples, 96 features + 1 label column                        |
| `cechy_all`            | 3399 × 99  | Full dataset: 96 features, 1 label, and 2 additional metadata columns       |

Each row corresponds to a segmented speech sample. The first 96 columns contain acoustic features, while the last column represents the emotion label. In `cechy_all`, additional columns may contain speaker IDs or class names.







