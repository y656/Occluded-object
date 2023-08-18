# Occluded-object
The occluded dataset creation process involved applying three distinct types of occlusions - Cloud, Rainy, and Foggy - to the high-resolution images extracted from the DOTA dataset. These occlusions were generated using the Python image-augmenter library, which allowed for the controlled introduction of weather-related visual impairments.

To manage the computational demands of working with high-resolution images, patches of the DOTA dataset were selected using the DOTA devkit. This patch-based approach helped reduce the input size while retaining the relevant information for the experiment.

In addition to the DOTA dataset, similar occlusions were also applied to images from the NWPU-VHR 10 dataset. This extended the scope of the experiment to evaluate the robustness of state-of-the-art (SOTA) object detection techniques, particularly focusing on the YOLO-V5 model.

The ultimate goal of this experiment was to assess the performance of the YOLO-V5 object detection model on these synthesized datasets with occlusions. The key metric used to evaluate the model's performance was the F1 score, which is a harmonic mean of precision and recall. Achieving an F1 score of 0.93 across all classes for the NWPU-VHR dataset indicates a high level of success in detecting objects under the occlusion conditions introduced by the Cloud, Rainy, and Foggy augmentations.

This experiment sheds light on the model's robustness and adaptability to challenging real-world scenarios, where adverse weather conditions can significantly impact the accuracy of object detection algorithms. The results obtained suggest that the YOLO-V5 model, when trained and evaluated on these occluded datasets, is capable of maintaining a high level of performance, making it a promising candidate for real-world applications where occlusions are prevalent.
