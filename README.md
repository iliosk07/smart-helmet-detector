 Smart Helmet Detector
Tier: 2 Student: Koffi Viglo and Erwin Cheng Course: ITAI 1378 – Introduction to Artificial Intelligence

 Problem Statement:

Many construction workers forget to wear helmets, which increases the risk of head injuries and death. Supervisors cannot always monitor everyone in real time.
Goal: Build an AI system that detects whether a worker is wearing a helmet using a camera.

 Proposed Solution:

Develop an object detection system that identifies:
	•	Workers wearing helmets
	•	Workers without helmets
If a person is detected without a helmet, the system can trigger an alert.

Technical Approach:

	•	Model: YOLOv8 (You Only Look Once, v8)
	•	Dataset: Roboflow public dataset — “Safety Helmet Detection”
	•	Environment: Google Colab (Python, free GPU)
	•	Libraries: ultralytics, opencv-python, matplotlib
	•	Training Steps:
	1	Import YOLOv8 model.
	2	Load dataset from Roboflow.
	3	Train and test the model.
	4	Evaluate accuracy and visualize predictions.

 System Pipeline:

 Camera →  YOLOv8 →  Detection →  Alert

	1	Capture image/video
	2	Detect persons and helmets
	3	Compare bounding boxes
	4	If a person has no helmet → send alert

Success Metrics:

Accuracy ≥ 85%
Precision ≥ 80%
Speed < 1 second per frame
False Alarms < 10%

Week-by-Week Plan:

Week 1:Research topic and find dataset on Roboflow
Week 2:Set up YOLOv8 in Google Colab and train model
Week 3:Evaluate and test model performance
Week 4:Finalize slides, documentation, and GitHub repo

 Challenges and Backup Plans:
Possible issues:
	•	Dataset too small → use Kaggle alternative.
	•	Model training too slow → use pretrained weights.
	•	Low accuracy → tune confidence threshold.

 Resources Needed:

	•	Google Colab (free GPU)
	•	Roboflow dataset link
	•	GitHub account
	•	Internet connection
	•	Laptop

 AI Tools and Assistance:

	•	ChatGPT used to rephrase and view grammar.
	•	YOLOv8 documentation for model configuration.
	•	Roboflow for dataset access and annotation.

 Folder Description:

	•	notebooks: Jupyter notebooks for code and testing.
	•	data: Small data samples and dataset info.
	•	docs: Proposal slides and reports.


