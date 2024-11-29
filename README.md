MediaPipe Auto-Annotated Dataset for Human Pose Estimation

Version 1.0

We are making the annotations and the corresponding code freely available for research purposes. If you would like to use the dataset for other purposes, please contact the authors.

Annotation Description

The annotations are stored in a JSON file with the following structure:

.annotations(image_idx)

	•	image.name - filename of the image
	•	pose_annotations(person_idx) - annotations for a person in the image
	•	head_rectangle - coordinates of the bounding box around the head
	•	scale - relative scale of the person in the image
	•	joint_positions - person-centric joint annotations:
	•	x, y - coordinates of each joint
	•	id - joint ID (e.g., 0 = right ankle, 1 = right knee, etc.)
	•	is_visible - visibility of the joint (1 = visible, 0 = not visible)
	•	activity - activity label for the image:
	•	name - activity name (e.g., “walking”, “jumping”)
	•	id - unique identifier for the activity
	•	video_idx - video index in the video list
	•	frame_sec - time in seconds when the frame occurs in the video

  Citing
  @inproceedings{andriluka14cvpr,
               author = {Mykhaylo Andriluka and Leonid Pishchulin and Peter Gehler and Schiele, Bernt}
               title = {2D Human Pose Estimation: New Benchmark and State of the Art Analysis},
               booktitle = {IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
               year = {2014},
               month = {June}
}