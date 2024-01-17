## FaceWatch backend
This repository contains the backend code for the Facewatch project, which is a health monitoring system using facial recognition and machine learning algorithms. The backend is responsible for accepting shared images from the user and updating the deep learning models with the new data. The server exposes an endpoint that Facewatch uses to send images. When a new image is received, it is added to the training data, and the deep learning models are retrained with the new data. The updated model weights are then added to the model.

To ensure efficient model updates, the version control "git" is used to track changes in the model weights. This allows the user to download only the changes, rather than the entire model, which can be time-consuming and resource-intensive.

The backend server flow
![image](https://github.com/abdelrahmanfekri/facewatchbackend/assets/84510558/5be74791-5137-4a5d-b5f5-27e369ff82cb)


To get started with the backend project, follow the installation and setup instructions below.

## Installation

Follow these steps to set up the backend project:

1. **Clone the Repository:**
2. **Create Virtual Environment:**

   ```bash
   python -m venv venv
   ```

3. **Activate Virtual Environment:**

   On Windows:

   ```bash
   venv\Scripts\activate
   ```

   On macOS/Linux:

   ```bash
   source venv/bin/activate
   ```

4. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

5. **Set Up Database:**

   ```bash
   python manage.py migrate
   ```

6. **Create Superuser (Optional):**

   ```bash
   python manage.py createsuperuser
   ```

7. **Run the Development Server:**

   ```bash
   python manage.py runserver
   ```

   Access the Django admin interface at http://localhost:8000/admin/ and the main application at http://localhost:8000/.

