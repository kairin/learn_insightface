# learn_insightface

from their recent release: https://github.com/deepinsight/inswapper-512-live


> ###Evaluation Metric Explanation:
> Similarity: The similarity between the generated face and the source face is evaluated using a third-party, high-precision face recognition model. The similarity score is calculated using the cosine similarity between the feature embeddings of the source and output images, scaled to a range of 0-100, where higher scores indicate greater similarity;

> Realism: This metric evaluates the realism and clarity of the generated face. We employ a comprehensive evaluation framework that combines the FID score, custom-designed metrics for facial clarity, and human perceptual evaluation. The score ranges from 0 to 100, with higher scores indicating a more realistic and clear result. We used a test set consisting of hundreds of high-resolution facial images, and randomly resized between 160x160 and 640x640 pixels in testing time;

> Attributes: This metric assesses the correlation between the attributes of the generated face and the target face, including factors such as pose, gaze direction, expression, etc. **We employ third-party facial attribute models to extract feature representations of both the generated and target images**. The similarities between these feature vectors are then computed to obtain the final metric score, which ranges from 0 to 100, with higher scores indicating better attribute alignment.
