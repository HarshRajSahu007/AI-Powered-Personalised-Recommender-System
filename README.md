# AI-Powered-Personalised-Recommender-System
Creating A scalable System that recommends personalised content/products to users based on the interaction history. It can be tailored for e-commerce, video streaming, or education platforms.

# TECH STACK AND KEY FEATURES:

# PYTORCH:
    1) Use PyTorch to develop a recommendation model (e.g., collaborative filtering with embeddings or neural matrix factorization).

    2) Train the model on user-item interaction data.

# TensorFlow:
    Convert the trained PyTorch model to ONNX and load it into TensorFlow Serving for efficient production deployment.

# FastAPI :
    Develop APIs to:
    1) Fetch recommendations for users.

    2) Handle user interactions (like rating a product or clicking on content).

    3) Retrieve user and item metadata from the database.

# PostgreSQL :
    1) Store user profiles, item details, and interaction data in a PostgreSQL database.
    
    2) Use the database for batch and online training/updating of recommendations.

# Git Modules :
    Organize the project into multiple repositories:
        1) Frontend Module: (optional) If you want a UI for testing.

        2) Backend Module: For FastAPI and database integration.

        3) ML Models Module: For the PyTorch training scripts.

        4) Deployment Module: Dockerize the application and manage TensorFlow Serving setup.


# Project Workflow:

    1) Data Processing :
        Simulate or use a dataset like MovieLens for user-item interactions.

        Preprocess data for training and testing.
    2) Model Training :
        Build a recommendation model using PyTorch.

        Save the model and convert it to ONNX for deployment.
    3) API Development :
        Create APIs using FastAPI to interact with the recommendation system.
        Include endpoints for:
            User interaction recording.

            Fetching recommendations.

            Updating user preferences.
    4) Database Integration
        Use PostgreSQL to manage user and item data.

        Write SQL queries for batch data aggregation and insights.
    5) Deployment
        Deploy the backend using Docker and integrate TensorFlow Serving for the trained model.

        Use FastAPI as a gateway between users and the model.



# Stretch Goals:

    1) Scalability: Use Kafka or RabbitMQ for streaming real-time user interactions.

    2) Visualization: Add a frontend to display recommendations.

    3) Advanced Models: Implement a hybrid recommender using PyTorch and TensorFlow (e.g., combining collaborative filtering and     content-based methods).