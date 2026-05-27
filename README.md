**Smart Crowd Panic Detection & Surveillance System Using AI and Computer Vision**

The Smart Crowd Panic Detection & Surveillance System is an advanced Artificial Intelligence based real-time monitoring system developed using Computer Vision, Deep Learning,
and Motion Analysis technologies. The main purpose of this project is to monitor crowded public areas and automatically detect dangerous situations such as crowd panic, 
overcrowding, abnormal movement, and stampede risks. In many public places like railway stations, airports, stadiums, temples, concerts, shopping malls, and festivals, 
managing large crowds manually becomes extremely difficult. Traditional CCTV systems only record video footage and require human operators to continuously monitor multiple 
screens, which often leads to delayed responses during emergency situations. When panic spreads inside a crowd, people start moving rapidly in different directions, creating 
chaos that may result in injuries, accidents, or loss of lives. This project aims to solve these real-world problems by introducing an intelligent automated surveillance 
system capable of analyzing crowd behavior in real time and generating emergency alerts before situations become critical.

The system is developed using Python as the core programming language along with several powerful libraries and frameworks such as OpenCV, YOLOv8, PyTorch, NumPy, and SciPy.
OpenCV is used for video capturing, frame processing, image manipulation, drawing bounding boxes, motion analysis, and displaying the output video stream. YOLOv8, which
stands for “You Only Look Once,” is a deep learning based object detection model used to detect humans in real time with high speed and accuracy. The model processes 
video frames and generates bounding boxes around detected persons. PyTorch is used as the backend deep learning framework for executing the YOLO model and enabling 
GPU acceleration for faster processing. NumPy is used for mathematical computations, matrix operations, and numerical processing, while SciPy is used for Gaussian filtering 
and heatmap smoothing to generate crowd density visualizations

The working process of the system begins with capturing video from a webcam, CCTV camera, or prerecorded video file. The video is divided into individual frames, and 
each frame is passed to the YOLOv8 model for person detection. Once humans are detected, the system tracks each individual by assigning unique IDs using an object tracking 
mechanism. The movement of every person is continuously monitored by calculating changes in position across consecutive frames. The speed and direction of movement are
analyzed to identify sudden abnormal movement patterns that may indicate panic situations. The project also uses Optical Flow analysis, specifically the Farneback Optical Flow 
algorithm, to analyze motion patterns between consecutive frames. Optical Flow helps the system understand how the crowd is moving collectively by measuring motion vectors, 
movement intensity, and directional flow. If people begin moving rapidly in different directions, the system interprets this as chaotic behavior and increases the panic score.

The project further calculates crowd density and motion entropy to evaluate the overall crowd condition. Heatmaps are generated using Gaussian filtering techniques to visually
represent crowded areas and panic hotspots. The system combines multiple parameters such as movement speed, crowd density, and motion entropy to calculate a panic score. 
Based on this score, the crowd condition is classified into different states such as NORMAL, ALERT, PANIC RISK, and MASS PANIC. When the panic score exceeds predefined 
threshold values, the system automatically generates emergency warnings on the screen, helping authorities respond quickly and prevent stampedes or crowd disasters.

This project provides several important advantages in real-world applications. It reduces the need for continuous human monitoring, improves response time during emergencies,
and enhances public safety in crowded environments. The system can be integrated into smart city surveillance infrastructure, public transportation systems, event management 
systems, and disaster management applications. It is highly useful for monitoring large public gatherings where crowd control and safety are critical. The project 
demonstrates the practical application of Artificial Intelligence and Computer Vision in solving real-world public safety challenges through intelligent surveillance and 
automated crowd behavior analysis.
