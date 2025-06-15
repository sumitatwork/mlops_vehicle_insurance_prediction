<div id="top">

<!-- HEADER STYLE: CLASSIC -->
<div align="center">

<img src="mlops_vehicle_insurance_prediction.png" width="30%" style="position: relative; top: 0; right: 0;" alt="Project Logo"/>

# MLOPS_VEHICLE_INSURANCE_PREDICTION

<em>Accelerating Insurance Innovation Through Smarter Predictions</em>

<!-- BADGES -->
<img src="https://img.shields.io/github/license/sumitatwork/mlops_vehicle_insurance_prediction?style=flat&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
<img src="https://img.shields.io/github/last-commit/sumitatwork/mlops_vehicle_insurance_prediction?style=flat&logo=git&logoColor=white&color=0080ff" alt="last-commit">
<img src="https://img.shields.io/github/languages/top/sumitatwork/mlops_vehicle_insurance_prediction?style=flat&color=0080ff" alt="repo-top-language">
<img src="https://img.shields.io/github/languages/count/sumitatwork/mlops_vehicle_insurance_prediction?style=flat&color=0080ff" alt="repo-language-count">

<em>Built with the tools and technologies:</em>

<img src="https://img.shields.io/badge/Markdown-000000.svg?style=flat&logo=Markdown&logoColor=white" alt="Markdown">
<img src="https://img.shields.io/badge/TOML-9C4121.svg?style=flat&logo=TOML&logoColor=white" alt="TOML">
<img src="https://img.shields.io/badge/scikitlearn-F7931E.svg?style=flat&logo=scikit-learn&logoColor=white" alt="scikitlearn">
<img src="https://img.shields.io/badge/FastAPI-009688.svg?style=flat&logo=FastAPI&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/NumPy-013243.svg?style=flat&logo=NumPy&logoColor=white" alt="NumPy">
<br>
<img src="https://img.shields.io/badge/Docker-2496ED.svg?style=flat&logo=Docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/Plotly-3F4F75.svg?style=flat&logo=Plotly&logoColor=white" alt="Plotly">
<img src="https://img.shields.io/badge/pandas-150458.svg?style=flat&logo=pandas&logoColor=white" alt="pandas">
<img src="https://img.shields.io/badge/YAML-CB171E.svg?style=flat&logo=YAML&logoColor=white" alt="YAML">

</div>
<br>

---

## Table of Contents

- [Overview](#overview)
- [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
    - [Usage](#usage)
    - [Testing](#testing)
- [Features](#features)
- [Project Structure](#project-structure)
    - [Project Index](#project-index)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgment](#acknowledgment)

---

## Overview

mlops_vehicle_insurance_prediction is a robust MLOps platform tailored for deploying vehicle insurance risk models. It orchestrates data ingestion, validation, transformation, model training, evaluation, and deployment, all within a scalable and modular architecture. The project emphasizes seamless integration with cloud storage, databases, and web interfaces, enabling developers to build, manage, and deploy machine learning solutions efficiently.

**Why mlops_vehicle_insurance_prediction?**

This project simplifies the complexities of deploying ML models in production environments. The core features include:

- 🧩 **🔧 Data Pipeline Automation:** Streamlines data ingestion from MongoDB, validation, and transformation workflows.
- 🚀 **📈 Model Training & Evaluation:** Facilitates training, performance assessment, and intelligent model versioning.
- ☁️ **🌐 Cloud & Database Integration:** Connects effortlessly with AWS S3 and MongoDB for scalable data management.
- 🖥️ **🎨 Web Interface:** Provides an intuitive web app for predictions, model management, and user interaction.
- 🐳 **🛠️ Containerized Deployment:** Ensures consistent environments across development and production.
- 🔄 **🔍 Modular Architecture:** Promotes maintainability, scalability, and clear artifact tracking.

---

## Features

|      | Component            | Details                                                                                     |
| :--- | :------------------- | :------------------------------------------------------------------------------------------ |
| ⚙️  | **Architecture**     | <ul><li>Modular design separating data ingestion, preprocessing, modeling, and deployment</li><li>Utilizes a pipeline approach with clear stages</li></ul> |
| 🔩 | **Code Quality**     | <ul><li>Consistent code style adhering to PEP8</li><li>Type hints with mypy for static type checking</li><li>Structured project layout with dedicated directories</li></ul> |
| 📄 | **Documentation**    | <ul><li>Comprehensive README with project overview and setup instructions</li><li>Configuration schemas in `schema.yaml` and `model.yaml`</li><li>Jupyter notebooks for exploratory analysis</li></ul> |
| 🔌 | **Integrations**     | <ul><li>FastAPI for serving models via REST API</li><li>Docker for containerization</li><li>AWS SDK (`boto3`) for cloud storage and resource management</li><li>MongoDB (`pymongo`) for data persistence</li></ul> |
| 🧩 | **Modularity**       | <ul><li>Separate modules for data processing, feature engineering, model training, and deployment</li><li>Configurable via YAML schemas</li></ul> |
| 🧪 | **Testing**          | <ul><li>Unit tests with `pytest` (implied by structure)</li><li>Type checks with `mypy`</li><li>Test data and mock objects likely used for validation</li></ul> |
| ⚡️  | **Performance**      | <ul><li>Use of optimized libraries like `numpy`, `pandas`, `scikit-learn`</li><li>Model serialization for fast inference</li><li>Potential use of batch processing in pipelines</li></ul> |
| 🛡️ | **Security**         | <ul><li>Schema validation with `schema.yaml` to prevent invalid data</li><li>Secure API endpoints via FastAPI</li><li>Containerization reduces environment variability</li></ul> |
| 📦 | **Dependencies**     | <ul><li>Managed via `requirements.txt` and `pyproject.toml`</li><li>Includes ML libraries (`scikit-learn`, `imblearn`, `plotly`), cloud SDKs (`boto3`), and web frameworks (`fastapi`, `uvicorn`)</li></ul> |

---

## Project Structure

```sh
└── mlops_vehicle_insurance_prediction/
    ├── Dockerfile
    ├── LICENSE
    ├── README.md
    ├── app.py
    ├── config
    │   ├── model.yaml
    │   └── schema.yaml
    ├── crashcourse.txt
    ├── demo.py
    ├── notebook
    │   ├── data.csv
    │   ├── exp-notebook.ipynb
    │   └── mongoDB_demo.ipynb
    ├── projectflow.txt
    ├── pyproject.toml
    ├── requirements.txt
    ├── setup.py
    ├── src
    │   ├── __init__.py
    │   ├── cloud_storage
    │   ├── components
    │   ├── configuration
    │   ├── constants
    │   ├── data_access
    │   ├── entity
    │   ├── exception
    │   ├── logger
    │   ├── pipline
    │   └── utils
    ├── static
    │   └── css
    ├── template.py
    └── templates
        └── vehicledata.html
```

---

### Project Index

<details open>
	<summary><b><code>MLOPS_VEHICLE_INSURANCE_PREDICTION/</code></b></summary>
	<!-- __root__ Submodule -->
	<details>
		<summary><b>__root__</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ __root__</b></code>
			<table style='width: 100%; border-collapse: collapse;'>
			<thead>
				<tr style='background-color: #f8f9fa;'>
					<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
					<th style='text-align: left; padding: 8px;'>Summary</th>
				</tr>
			</thead>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/pyproject.toml'>pyproject.toml</a></b></td>
					<td style='padding: 8px;'>- Defines project metadata and dependencies for an MLOps platform focused on productionizing machine learning models<br>- It establishes the package structure, versioning, and required libraries, serving as the foundation for building, managing, and deploying scalable ML solutions within the overall architecture<br>- This configuration ensures consistent environment setup and streamlined project management.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/LICENSE'>LICENSE</a></b></td>
					<td style='padding: 8px;'>- Provides the licensing terms that govern the entire project, ensuring legal clarity and usage permissions<br>- It establishes the open-source MIT License under which the software is distributed, facilitating broad adoption, modification, and distribution within the projects architecture<br>- This foundational document supports the projects collaborative development and open-source ethos.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/projectflow.txt'>projectflow.txt</a></b></td>
					<td style='padding: 8px;'>- Provides foundational setup and orchestration for the entire machine learning pipeline, including project scaffolding, environment configuration, database integration, logging, exception handling, and cloud storage connectivity<br>- Facilitates seamless data ingestion from MongoDB, data validation, transformation, model training, evaluation, and deployment workflows, while ensuring infrastructure readiness on AWS and local development environments.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/README.md'>README.md</a></b></td>
					<td style='padding: 8px;'>- Provides the core functionality for deploying and managing vehicle insurance prediction models within the MLOps platform<br>- It orchestrates data ingestion, validation, transformation, model training, evaluation, and deployment, enabling seamless integration with cloud storage and databases<br>- Facilitates user interaction through a web interface, supporting scalable, end-to-end machine learning workflows in a modular architecture.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/Dockerfile'>Dockerfile</a></b></td>
					<td style='padding: 8px;'>- Builds a containerized environment optimized for deploying the application, ensuring consistent runtime conditions across development, testing, and production<br>- It encapsulates dependencies and configurations necessary for the service to operate reliably within the overall architecture, facilitating seamless deployment and scalability within the broader system infrastructure.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/crashcourse.txt'>crashcourse.txt</a></b></td>
					<td style='padding: 8px;'>- Defines project configuration and dependency management using pyproject.toml, streamlining Python packaging and build processes<br>- Facilitates centralized metadata, flexible build system support, and dependency linking, ensuring consistent environment setup<br>- Supports modern development workflows by replacing traditional setup.py and requirements.txt, enabling efficient project setup, dependency handling, and packaging within the overall architecture.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/demo.py'>demo.py</a></b></td>
					<td style='padding: 8px;'>- Facilitates execution of the training pipeline within the overall project architecture, orchestrating data processing, model training, and evaluation steps<br>- Serves as an entry point for initiating the machine learning workflow, ensuring seamless integration with logging and exception handling mechanisms to support robust and maintainable model development.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/app.py'>app.py</a></b></td>
					<td style='padding: 8px;'>- Facilitates vehicle insurance risk assessment by providing web endpoints for data input, model prediction, and training initiation<br>- Renders user interface, processes form data, and returns prediction results, integrating the machine learning pipeline within a FastAPI framework<br>- Supports seamless interaction between users and the predictive model, enabling both inference and model retraining in a cohesive architecture.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/requirements.txt'>requirements.txt</a></b></td>
					<td style='padding: 8px;'>- Defines project dependencies essential for data processing, machine learning, web API development, and cloud interactions<br>- Supports seamless integration of data analysis, model training, and deployment workflows within the overall architecture, ensuring consistent environment setup and facilitating scalable, reliable application development across various components.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/setup.py'>setup.py</a></b></td>
					<td style='padding: 8px;'>- Defines the package configuration and setup parameters for the project, enabling seamless installation and distribution of the codebase<br>- It specifies essential metadata and package discovery, ensuring that the entire project is correctly structured and accessible for development, testing, and deployment within the broader architecture.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/template.py'>template.py</a></b></td>
					<td style='padding: 8px;'>- Defines the projects foundational structure by creating necessary directories and placeholder files for a comprehensive machine learning pipeline<br>- It ensures all core components, including data ingestion, validation, transformation, model training, evaluation, deployment, and configuration, are properly organized, facilitating seamless development, maintenance, and scalability within the overall architecture.</td>
				</tr>
			</table>
		</blockquote>
	</details>
	<!-- notebook Submodule -->
	<details>
		<summary><b>notebook</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ notebook</b></code>
			<table style='width: 100%; border-collapse: collapse;'>
			<thead>
				<tr style='background-color: #f8f9fa;'>
					<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
					<th style='text-align: left; padding: 8px;'>Summary</th>
				</tr>
			</thead>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/notebook/exp-notebook.ipynb'>exp-notebook.ipynb</a></b></td>
					<td style='padding: 8px;'>- Summary of <code>notebook/exp-notebook.ipynb</code>This notebook serves as an experimental environment within the project, designed to facilitate exploratory data analysis, model development, and validation workflows<br>- It provides a flexible interface for testing hypotheses, visualizing data insights, and iterating on machine learning or analytical models before integrating them into the main codebase<br>- Overall, it acts as a sandbox for experimentation that supports the broader architectures goal of scalable, data-driven decision-making.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/notebook/mongoDB_demo.ipynb'>mongoDB_demo.ipynb</a></b></td>
					<td style='padding: 8px;'>- Facilitates the ingestion of vehicle insurance data into a MongoDB database, enabling efficient storage and retrieval for subsequent analysis or modeling<br>- Converts a pandas DataFrame into a suitable format, establishes a database connection, and uploads the data, supporting scalable data management within the overall machine learning or data processing architecture.</td>
				</tr>
			</table>
		</blockquote>
	</details>
	<!-- src Submodule -->
	<details>
		<summary><b>src</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ src</b></code>
			<!-- data_access Submodule -->
			<details>
				<summary><b>data_access</b></summary>
				<blockquote>
					<div class='directory-path' style='padding: 8px 0; color: #666;'>
						<code><b>⦿ src.data_access</b></code>
					<table style='width: 100%; border-collapse: collapse;'>
					<thead>
						<tr style='background-color: #f8f9fa;'>
							<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
							<th style='text-align: left; padding: 8px;'>Summary</th>
						</tr>
					</thead>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/data_access/proj1_data.py'>proj1_data.py</a></b></td>
							<td style='padding: 8px;'>- Provides functionality to extract entire MongoDB collections as cleaned pandas DataFrames, facilitating data access and analysis within the project<br>- It ensures seamless integration between the database and data processing workflows by handling data retrieval, preprocessing, and error management, supporting the broader data architecture of the application.</td>
						</tr>
					</table>
				</blockquote>
			</details>
			<!-- utils Submodule -->
			<details>
				<summary><b>utils</b></summary>
				<blockquote>
					<div class='directory-path' style='padding: 8px 0; color: #666;'>
						<code><b>⦿ src.utils</b></code>
					<table style='width: 100%; border-collapse: collapse;'>
					<thead>
						<tr style='background-color: #f8f9fa;'>
							<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
							<th style='text-align: left; padding: 8px;'>Summary</th>
						</tr>
					</thead>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/utils/main_utils.py'>main_utils.py</a></b></td>
							<td style='padding: 8px;'>- Provides utility functions for managing configuration, data serialization, and model persistence within the project<br>- Facilitates reading and writing YAML files, saving and loading numpy arrays, and serializing objects with dill, supporting seamless data handling and model management across the codebase<br>- Enhances robustness through exception handling, ensuring reliable data operations in the overall architecture.</td>
						</tr>
					</table>
				</blockquote>
			</details>
			<!-- configuration Submodule -->
			<details>
				<summary><b>configuration</b></summary>
				<blockquote>
					<div class='directory-path' style='padding: 8px 0; color: #666;'>
						<code><b>⦿ src.configuration</b></code>
					<table style='width: 100%; border-collapse: collapse;'>
					<thead>
						<tr style='background-color: #f8f9fa;'>
							<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
							<th style='text-align: left; padding: 8px;'>Summary</th>
						</tr>
					</thead>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/configuration/aws_connection.py'>aws_connection.py</a></b></td>
							<td style='padding: 8px;'>- Establishes a secure connection to AWS S3 by retrieving credentials from environment variables, enabling seamless interaction with S3 storage within the broader application architecture<br>- Facilitates centralized access to cloud storage resources, supporting data management, storage, and retrieval operations essential for the systems cloud-based functionalities.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/configuration/mongo_db_connection.py'>mongo_db_connection.py</a></b></td>
							<td style='padding: 8px;'>- Establishes a robust connection to the MongoDB database within the project architecture, enabling seamless data storage and retrieval<br>- It manages shared client instances to optimize resource usage and ensures secure, reliable connectivity through environment-configured credentials<br>- This component is fundamental for enabling database interactions across various modules, supporting the overall data-driven functionality of the system.</td>
						</tr>
					</table>
				</blockquote>
			</details>
			<!-- components Submodule -->
			<details>
				<summary><b>components</b></summary>
				<blockquote>
					<div class='directory-path' style='padding: 8px 0; color: #666;'>
						<code><b>⦿ src.components</b></code>
					<table style='width: 100%; border-collapse: collapse;'>
					<thead>
						<tr style='background-color: #f8f9fa;'>
							<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
							<th style='text-align: left; padding: 8px;'>Summary</th>
						</tr>
					</thead>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/components/model_evaluation.py'>model_evaluation.py</a></b></td>
							<td style='padding: 8px;'>- Facilitates comprehensive evaluation of trained machine learning models by comparing their performance against existing production models using F1 scores<br>- It preprocesses test data, loads models from storage, and determines whether the new model should replace the current one, ultimately generating an artifact that guides deployment decisions within the overall architecture.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/components/data_validation.py'>data_validation.py</a></b></td>
							<td style='padding: 8px;'>- Implements data validation procedures to ensure dataset integrity by verifying column counts and existence of required numerical and categorical features<br>- Facilitates early detection of schema discrepancies in training and testing data, generating validation reports to support reliable data ingestion and preprocessing within the overall pipeline architecture.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/components/data_ingestion.py'>data_ingestion.py</a></b></td>
							<td style='padding: 8px;'>- Facilitates data ingestion by exporting data from MongoDB into a feature store, then splitting it into training and testing datasets<br>- Supports the overall data pipeline by preparing and organizing raw data for subsequent modeling stages, ensuring data is accessible, structured, and ready for machine learning workflows within the project architecture.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/components/data_transformation.py'>data_transformation.py</a></b></td>
							<td style='padding: 8px;'>- Implements comprehensive data transformation workflows, including feature engineering, scaling, and encoding, to prepare raw data for modeling<br>- Integrates custom preprocessing steps with scalable pipelines, handles class imbalance with SMOTEENN, and saves transformed datasets and objects, ensuring consistent and robust data readiness within the overall architecture.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/components/model_trainer.py'>model_trainer.py</a></b></td>
							<td style='padding: 8px;'>- Implements model training and evaluation using a RandomForestClassifier, integrating data transformation artifacts and configuration settings<br>- It trains the model, assesses performance metrics, and saves the best-performing model, ensuring alignment with expected accuracy thresholds<br>- Facilitates seamless model deployment within the overall architecture by encapsulating training, evaluation, and persistence processes.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/components/model_pusher.py'>model_pusher.py</a></b></td>
							<td style='padding: 8px;'>- Handles deployment of the trained model by uploading it to an S3 bucket, ensuring the model is accessible for production use<br>- Integrates with evaluation artifacts and configuration settings to automate model pushing, facilitating seamless model versioning and deployment within the overall architecture.</td>
						</tr>
					</table>
				</blockquote>
			</details>
			<!-- pipline Submodule -->
			<details>
				<summary><b>pipline</b></summary>
				<blockquote>
					<div class='directory-path' style='padding: 8px 0; color: #666;'>
						<code><b>⦿ src.pipline</b></code>
					<table style='width: 100%; border-collapse: collapse;'>
					<thead>
						<tr style='background-color: #f8f9fa;'>
							<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
							<th style='text-align: left; padding: 8px;'>Summary</th>
						</tr>
					</thead>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/pipline/training_pipeline.py'>training_pipeline.py</a></b></td>
							<td style='padding: 8px;'>- Orchestrates the end-to-end training pipeline by coordinating data ingestion, validation, transformation, model training, evaluation, and deployment<br>- Ensures seamless progression through each stage, enabling automated and structured model development and deployment workflows within the overall architecture<br>- Facilitates robust, scalable, and maintainable machine learning lifecycle management.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/pipline/prediction_pipeline.py'>prediction_pipeline.py</a></b></td>
							<td style='padding: 8px;'>- Facilitates vehicle insurance risk prediction by transforming input features into a structured DataFrame and leveraging a pre-trained model for classification<br>- Integrates configuration management and logging to ensure robust predictions within the overall prediction pipeline, enabling seamless deployment of vehicle insurance risk assessments.</td>
						</tr>
					</table>
				</blockquote>
			</details>
			<!-- cloud_storage Submodule -->
			<details>
				<summary><b>cloud_storage</b></summary>
				<blockquote>
					<div class='directory-path' style='padding: 8px 0; color: #666;'>
						<code><b>⦿ src.cloud_storage</b></code>
					<table style='width: 100%; border-collapse: collapse;'>
					<thead>
						<tr style='background-color: #f8f9fa;'>
							<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
							<th style='text-align: left; padding: 8px;'>Summary</th>
						</tr>
					</thead>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/cloud_storage/aws_storage.py'>aws_storage.py</a></b></td>
							<td style='padding: 8px;'>- Provides a comprehensive interface for managing AWS S3 storage, enabling file existence checks, data uploads, model loading, and CSV processing<br>- Facilitates seamless interaction with S3 buckets for data storage, retrieval, and organization, supporting data-driven workflows and machine learning model deployment within the broader cloud-based architecture.</td>
						</tr>
					</table>
				</blockquote>
			</details>
			<!-- entity Submodule -->
			<details>
				<summary><b>entity</b></summary>
				<blockquote>
					<div class='directory-path' style='padding: 8px 0; color: #666;'>
						<code><b>⦿ src.entity</b></code>
					<table style='width: 100%; border-collapse: collapse;'>
					<thead>
						<tr style='background-color: #f8f9fa;'>
							<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
							<th style='text-align: left; padding: 8px;'>Summary</th>
						</tr>
					</thead>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/entity/estimator.py'>estimator.py</a></b></td>
							<td style='padding: 8px;'>- Defines core components for model inference, including a mapping for target labels and a wrapper class that applies preprocessing and generates predictions using trained models<br>- Facilitates seamless deployment of machine learning models by ensuring consistent data transformation and prediction workflows within the overall architecture.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/entity/config_entity.py'>config_entity.py</a></b></td>
							<td style='padding: 8px;'>- Defines configuration schemas for the vehicle prediction pipeline, centralizing paths, parameters, and settings across data ingestion, validation, transformation, model training, evaluation, and deployment stages<br>- Facilitates consistent, organized management of artifacts and parameters, ensuring seamless integration and reproducibility within the overall machine learning architecture.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/entity/artifact_entity.py'>artifact_entity.py</a></b></td>
							<td style='padding: 8px;'>- Defines data structures representing key artifacts throughout the machine learning pipeline, including data ingestion, validation, transformation, model training, evaluation, and deployment<br>- These classes facilitate consistent tracking and management of process outputs, ensuring seamless integration and communication across different stages of the architecture.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/src/entity/s3_estimator.py'>s3_estimator.py</a></b></td>
							<td style='padding: 8px;'>- Provides mechanisms to manage machine learning models stored in AWS S3, including saving, loading, and verifying model presence<br>- Facilitates seamless integration of model retrieval and prediction within the broader system architecture, enabling scalable and efficient deployment of predictive capabilities in cloud-based environments<br>- Ensures robust model management aligned with cloud storage best practices.</td>
						</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<!-- templates Submodule -->
	<details>
		<summary><b>templates</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ templates</b></code>
			<table style='width: 100%; border-collapse: collapse;'>
			<thead>
				<tr style='background-color: #f8f9fa;'>
					<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
					<th style='text-align: left; padding: 8px;'>Summary</th>
				</tr>
			</thead>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/templates/vehicledata.html'>vehicledata.html</a></b></td>
					<td style='padding: 8px;'>- Provides a user interface for vehicle insurance prediction by collecting relevant customer and vehicle data, enabling users to submit inputs for risk assessment<br>- Facilitates model training initiation and displays prediction results, integrating seamlessly into the web application architecture to support insurance decision-making processes.</td>
				</tr>
			</table>
		</blockquote>
	</details>
	<!-- config Submodule -->
	<details>
		<summary><b>config</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ config</b></code>
			<table style='width: 100%; border-collapse: collapse;'>
			<thead>
				<tr style='background-color: #f8f9fa;'>
					<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
					<th style='text-align: left; padding: 8px;'>Summary</th>
				</tr>
			</thead>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/config/model.yaml'>model.yaml</a></b></td>
					<td style='padding: 8px;'>- Defines the model configuration parameters essential for the applications machine learning components, ensuring consistent setup and deployment across different environments<br>- Serves as a centralized reference for model architecture, hyperparameters, and related settings, facilitating seamless integration within the overall system architecture and supporting reliable, reproducible model training and inference workflows.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/master/config/schema.yaml'>schema.yaml</a></b></td>
					<td style='padding: 8px;'>- Defines the data schema for the project, specifying feature types, transformations, and columns to include or exclude<br>- Facilitates consistent data processing and feature engineering across the architecture, ensuring accurate model training and evaluation within the broader machine learning pipeline<br>- Supports data validation and transformation workflows integral to the systems predictive modeling objectives.</td>
				</tr>
			</table>
		</blockquote>
	</details>
</details>

---

## Getting Started

### Prerequisites

This project requires the following dependencies:

- **Programming Language:** Python
- **Package Manager:** Pip
- **Container Runtime:** Docker

### Installation

Build mlops_vehicle_insurance_prediction from the source and install dependencies:

1. **Clone the repository:**

    ```sh
    ❯ git clone https://github.com/sumitatwork/mlops_vehicle_insurance_prediction
    ```

2. **Navigate to the project directory:**

    ```sh
    ❯ cd mlops_vehicle_insurance_prediction
    ```

3. **Install the dependencies:**

**Using [docker](https://www.docker.com/):**

```sh
❯ docker build -t sumitatwork/mlops_vehicle_insurance_prediction .
```
**Using [pip](https://pypi.org/project/pip/):**

```sh
❯ pip install -r requirements.txt
```

### Usage

Run the project with:

**Using [docker](https://www.docker.com/):**

```sh
docker run -it {image_name}
```
**Using [pip](https://pypi.org/project/pip/):**

```sh
python {entrypoint}
```

### Testing

Mlops_vehicle_insurance_prediction uses the {__test_framework__} test framework. Run the test suite with:

**Using [docker](https://www.docker.com/):**

```sh
echo 'INSERT-TEST-COMMAND-HERE'
```
**Using [pip](https://pypi.org/project/pip/):**

```sh
pytest
```

---

## Roadmap

- [X] **`Task 1`**: <strike>Implement feature one.</strike>
- [ ] **`Task 2`**: Implement feature two.
- [ ] **`Task 3`**: Implement feature three.

---

## Contributing

- **💬 [Join the Discussions](https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/discussions)**: Share your insights, provide feedback, or ask questions.
- **🐛 [Report Issues](https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/issues)**: Submit bugs found or log feature requests for the `mlops_vehicle_insurance_prediction` project.
- **💡 [Submit Pull Requests](https://github.com/sumitatwork/mlops_vehicle_insurance_prediction/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.

<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your github account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone https://github.com/sumitatwork/mlops_vehicle_insurance_prediction
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to github**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.
8. **Review**: Once your PR is reviewed and approved, it will be merged into the main branch. Congratulations on your contribution!
</details>

<details closed>
<summary>Contributor Graph</summary>
<br>
<p align="left">
   <a href="https://github.com{/sumitatwork/mlops_vehicle_insurance_prediction/}graphs/contributors">
      <img src="https://contrib.rocks/image?repo=sumitatwork/mlops_vehicle_insurance_prediction">
   </a>
</p>
</details>

---

## License

Mlops_vehicle_insurance_prediction is protected under the [LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.

---

## Acknowledgments

- Credit `contributors`, `inspiration`, `references`, etc.

<div align="left"><a href="#top">⬆ Return</a></div>

---
