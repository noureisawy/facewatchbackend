## FaceWatch backend
This repository contains the backend code for the Facewatch project, which is a health monitoring system using facial recognition and machine learning algorithms. The backend is responsible for accepting shared images from the user and updating the deep learning models with the new data. The server exposes an endpoint that Facewatch uses to send images. When a new image is received, it is added to the training data, and the deep learning models are retrained with the new data. The updated model weights are then added to the model.

To ensure efficient model updates, the version control "git" is used to track changes in the model weights. This allows the user to download only the changes, rather than the entire model, which can be time-consuming and resource-intensive.

The backend server flow is illustrated in the "Backend Server Flow" diagram in the repository.

To get started with the backend project, follow the installation and setup instructions below.

Installation and Setup:
1. Clone the repository to your local machine.
2. Install the required dependencies using the package manager of your choice (e.g., pip, conda).
3. Set up a virtual environment for the project to manage dependencies.
4. Run the backend server using the provided scripts or commands.

Contributing:
If you would like to contribute to the backend project, please follow the guidelines outlined in the CONTRIBUTING.md file in the repository.
