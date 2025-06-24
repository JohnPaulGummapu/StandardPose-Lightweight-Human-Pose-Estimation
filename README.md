# StandardPose-Lightweight-Human-Pose-Estimation

This Python script utilizes the MediaPipe Pose model to detect and classify human poses in static images, specifically distinguishing between Sitting and Standing positions.

The model is configured to operate in static image mode. It processes a given image to detect pose landmarks using MediaPipe. To classify the pose, the script calculates joint angles—particularly at the knee and hip—by referencing key landmarks such as the shoulder, hip, knee, and ankle. Based on these computed angles, the script labels the image as Standing, Sitting, or Unknown.

The annotated image is then saved in the Outputs directory with a proc_ prefix.

An optional visualization mode is available to display pose landmarks directly on the input image, aiding in understanding and debugging.

This tool is ideal for analyzing individual images to automatically determine pose classification using joint geometry and MediaPipe's robust landmark detection system.
