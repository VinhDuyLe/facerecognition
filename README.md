
# Face Recognition using Siamese Neural Networks
## Implementation details
1. Tools/dependencies: TensorFlow for model building and OpenCV for image processing
2. Data Collection and Preprocessing:
- Used the Labeled Faces in the Wild dataset for negative samples and webcam-captured images for positive and anchor samples.
- Data augmentation like brightness and contrast adjustments for robustness.
3. Model Engineering:
- Employed a Siamese Network with two identical CNNs converging into a distance metric layer for feature comparison.
- Utilized an L1 Distance layer for similarity assessment between feature vectors.
4. Training and Evaluation:
- Trained on image pairs to distinguish between similar and dissimilar faces using binary cross-entropy loss and Adam optimizer.
- Evaluated model performance using precision, recall, and accuracy metrics.
5. Real-Time Testing:
- Integrated a webcam for live image capture and verification against a dataset.
- Provided immediate match likelihood feedback for verification

## Sources
- [Siamese Neural Networks for One-shot Image Recognition](https://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf)
- [Labeled Faces in the Wild](http://vis-www.cs.umass.edu/lfw/) (all images as gzipped tar file)
