Assignment 1 - Sameera SHEIK, Mugil KOLANCHI
# Voice Classification using SVM
The objective is to classify two voices of Sameera and Mugil using SVM.

# Dataset
The audio data is created by the voices of Sameera and Mugil, by reading the same paragraphs. 

### Text 1:
“The North Wind and the Sun were disputing which was the stronger, when a traveler came along wrapped in a warm cloak. They agreed that the one who first succeeded in making the traveler take his cloak off should be considered stronger than the other. Then the North Wind blew as hard as he could, but the more he blew the more closely did the traveler fold his cloak around him; and at last the North Wind gave up the attempt. Then the Sun shone out warmly, and immediately the traveler took off his cloak. And so the North Wind was obliged to confess that the Sun was the stronger of the two.”

### Text 2:
"This is because there is less scattering of blue light as the atmospheric path length and consequently the degree of scattering of the incoming radiation is reduced. For the same reason, the sun appears to be whiter and less orange-coloured as the observer's altitude increases; this is because a greater proportion of the sunlight comes directly to the observer's eye. Figure 5.7 is a schematic representation of the path of electromagnetic energy in the visible spectrum as it travels from the sun to the Earth and back again towards a sensor mounted on an orbiting satellite. The paths of waves representing energy prone to scattering (that is, the shorter wavelengths) as it travels from sun to Earth are shown. To the sensor it appears that all the energy has been reflected from point P on the ground whereas, in fact, it has not, because some has been scattered within the atmosphere and has never reached the ground at all"

# Feature Extraction
- Each audio is sliced into 5s time period.
- Audio features like chroma_stft, rmse, spectral_centroid, spectral_bandwidth, rolloff,zero_crossing_rate and mfcc are extracted from the subsliced audios using librosa and used as the input to the model

# Model
SVM without any kernel is used for the training and prediction