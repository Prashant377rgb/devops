FastAPI Math API

📌 Overview

This FastAPI project provides a simple API for performing basic mathematical operations such as addition, subtraction, and multiplication. The API is designed for quick calculations and is tested using automated scripts to ensure reliability. Additionally, it integrates seamlessly with GitHub Actions for continuous integration and deployment.

🚀 Features

Perform basic math operations: Addition, subtraction, and multiplication.

Built with FastAPI: A high-performance Python web framework known for its speed and efficiency.

Automated Testing: Uses pytest to validate API functionality.

CI/CD Pipeline: Integrated with GitHub Actions for continuous testing and deployment.

Lightweight & Fast: Minimal dependencies with a fast response time.

RESTful API Design: Follows best practices for REST API development.

Scalability: Can be extended with authentication, databases, and additional functionality.

🛠️ Setup Instructions

1️⃣ Install Dependencies

Ensure you have Python installed on your system. Then, install the required dependencies using the following command:

pip install fastapi uvicorn requests pytest

2️⃣ Run the FastAPI Server

Start the API server using the following command:

python math_api.py

The server will be available at: http://localhost:8000

3️⃣ Test the API Endpoints

You can test the API endpoints using a web browser, Postman, or curl:

Addition: http://localhost:8000/sum/3/5 → Response: { "calculated_sum": 8 }

Subtraction: http://localhost:8000/difference/9/4 → Response: { "calculated_difference": 5 }

Multiplication: http://localhost:8000/product/3/4 → Response: { "calculated_product": 12 }

For command-line testing using curl:

curl http://localhost:8000/sum/3/5

🔬 Automated Testing

4️⃣ Run Tests Using Pytest

To verify API functionality, execute the following command:

pytest test_my_api.py

If all tests pass, you will see output similar to:

============================= test session starts =============================
collected 3 items

✅ test_my_api.py ... [PASS]

============================== 3 passed in 0.5s ==============================

⚙️ GitHub Actions CI/CD

This project includes a GitHub Actions workflow to automate testing on every code push and pull request. The workflow is defined in .github/workflows/test.yml.

 Steps in the CI/CD Pipeline:

Checkout Code – Pulls the latest code from the repository.

Set Up Python – Installs Python and all dependencies.

Start FastAPI Server – Runs the API in the background.

Run Tests – Executes pytest to validate all API endpoints.

Generate Reports – Outputs test results and logs.

 Running the Pipeline

To trigger the pipeline, commit and push your changes to the repository:

git add .
git commit -m "Updated FastAPI project with CI/CD"
git push origin main

Once pushed, navigate to the Actions tab in your GitHub repository to monitor workflow execution and test results.

 Future Enhancements

 Add database integration (PostgreSQL/MongoDB) for storing calculations.

 Implement authentication (JWT/OAuth2) for secure API access.

 Enhance error handling and logging mechanisms.

 Add performance testing with locust.io to benchmark API efficiency.

 Deploy to cloud platforms like AWS, GCP, or Heroku.

 Implement caching for improved response times.

 Add Docker support for easy deployment.

📝 Author

Developed and maintained by Prashant Srivastava. 🚀

💡 Contributions and suggestions are welcome! Feel free to open an issue or submit a pull request to enhance the project further.

