<p align="center">
    <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" align="center" width="30%">
</p>
<p align="center"><h1 align="center">WHEAT_YIELD_PREDICTION</h1></p>
<p align="center">
	<em>Harvesting Future Yields with Data Today!</em>
</p>
<p align="center">
	<img src="https://img.shields.io/github/license/dgebenicolas/Wheat_Yield_Prediction?style=default&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
	<img src="https://img.shields.io/github/last-commit/dgebenicolas/Wheat_Yield_Prediction?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/dgebenicolas/Wheat_Yield_Prediction?style=default&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/dgebenicolas/Wheat_Yield_Prediction?style=default&color=0080ff" alt="repo-language-count">
</p>
<p align="center"><!-- default option, no dependency badges. -->
</p>
<p align="center">
	<!-- default option, no dependency badges. -->
</p>
<br>

##  Table of Contents

- [ Overview](#-overview)
- [ Features](#-features)
- [ Project Structure](#-project-structure)
  - [ Project Index](#-project-index)
- [ Getting Started](#-getting-started)
  - [ Prerequisites](#-prerequisites)
  - [ Installation](#-installation)
  - [ Usage](#-usage)
  - [ Testing](#-testing)
- [ Project Roadmap](#-project-roadmap)
- [ Contributing](#-contributing)
- [ License](#-license)
- [ Acknowledgments](#-acknowledgments)

---

##  Overview

The WheatYieldPrediction project is a powerful tool for predicting wheat yields using machine learning. It leverages environmental data, soil properties, and vegetation indices to provide accurate forecasts. This open-source project is invaluable for farmers, agricultural researchers, and policy makers, offering insights to optimize crop production and support sustainable farming practices.

---

##  Features

|      | Feature         | Summary       |
| :--- | :---:           | :---          |
| ⚙️  | **Architecture**  | <ul><li>The project uses a modular architecture with separate files for utility functions (`utils.py`), application entry point (`app.py`), and data collection and processing (`Data_Collection_GEE.ipynb`, `Wheat_Yield_Data_Processing.ipynb`).</li><li>The project uses Jupyter notebooks for data collection, processing, exploratory data analysis, and machine learning tasks.</li><li>The project uses a GeoJSON file (`All Fields Polygons.geojson`) to store and share geographic data.</li></ul> |
| 🔩 | **Code Quality**  | <ul><li>The code is well-structured and modular, with separate files for different functionalities.</li><li>The project uses Python, a language known for its readability and simplicity.</li><li>The project uses a variety of libraries to ensure code efficiency and functionality.</li></ul> |
| 📄 | **Documentation** | <ul><li>The project uses Jupyter notebooks, which allow for inline documentation and explanation of code.</li><li>The project includes a `requirements.txt` file, which outlines the necessary libraries for the project.</li><li>However, the project seems to lack a comprehensive README or other high-level documentation.</li></ul> |
| 🔌 | **Integrations**  | <ul><li>The project integrates with Google Earth Engine for data collection (`Data_Collection_GEE.ipynb`).</li><li>The project uses `pip` as its package manager, as indicated by the `requirements.txt` file.</li><li>The project integrates with various Python libraries for data manipulation, machine learning, data visualization, and scientific computing.</li></ul> |
| 🧩 | **Modularity**    | <ul><li>The project is highly modular, with separate files for different functionalities.</li><li>The project uses utility functions (`utils.py`) to handle data preprocessing, validation, and transformation tasks.</li><li>The project uses Jupyter notebooks for different data processing and analysis tasks.</li></ul> |
| 🧪 | **Testing**       | <ul><li>The project does not seem to include any specific testing frameworks or test cases.</li><li>However, the use of Jupyter notebooks allows for interactive testing and debugging of code.</li></ul> |
| ⚡️  | **Performance**   | <ul><li>The project uses `lightgbm`, a gradient boosting framework that is known for its high performance and efficiency.</li><li>The project uses `numpy` and `pandas` for efficient data manipulation.</li><li>The project uses `scipy` for efficient scientific computing.</li></ul> |
| 🛡️ | **Security**      | <ul><li>The project does not seem to include any specific security measures or considerations.</li><li>However, the use of `pip` for package management helps ensure that all dependencies are up-to-date and secure.</li></ul> |

---

##  Project Structure

```sh
└── Wheat_Yield_Prediction/
    ├── All Fields Polygons.geojson
    ├── Notebooks
    │   ├── Data_Collection_GEE.ipynb
    │   ├── Exploratory_Data_Analysis.ipynb
    │   ├── Machine_Learning.ipynb
    │   └── Wheat_Yield_Data_Processing.ipynb
    ├── README.md
    ├── app.py
    ├── lgbfit_new.txt
    ├── requirements.txt
    ├── test.csv
    └── utils.py
```


###  Project Index
<details open>
	<summary><b><code>WHEAT_YIELD_PREDICTION/</code></b></summary>
	<details> <!-- __root__ Submodule -->
		<summary><b>__root__</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/utils.py'>utils.py</a></b></td>
				<td>- The 'utils.py' file serves as a utility module for a data processing pipeline<br>- It primarily handles data preprocessing, validation, and transformation tasks<br>- The code ensures that the input data is in the correct format, removes outliers, standardizes numerical features, and applies one-hot encoding to categorical features<br>- It also maps specific product names to broader categories for easier analysis.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/app.py'>app.py</a></b></td>
				<td>- App.py serves as the main entry point for a crop yield prediction application<br>- It integrates various functionalities including data preprocessing, model loading, user input handling, and data visualization<br>- The application predicts crop yields based on various features like weather data, soil properties, and vegetation indices, and presents the results in a user-friendly interface.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/lgbfit_new.txt'>lgbfit_new.txt</a></b></td>
				<td>- The file `lgbfit_new.txt` is part of a larger codebase that is structured for a machine learning project<br>- This particular file is used for configuring a LightGBM model, a gradient boosting framework that uses tree-based learning algorithms, for a regression task<br>- The file specifies the version of the model, the number of classes, the number of trees per iteration, the label index, and the maximum feature index<br>- It also lists the feature names that the model will use for training<br>- These features include various environmental factors such as NDVI (Normalized Difference Vegetation Index) and relative humidity, which suggests that the project might be related to environmental or climate studies<br>- In the context of the entire codebase, this file is crucial for setting up the machine learning model that likely drives the core functionality of the project.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/requirements.txt'>requirements.txt</a></b></td>
				<td>- Requirements.txt outlines the necessary libraries for the project, including pandas, numpy, lightgbm, streamlit, scikit-learn, plotly, and scipy<br>- These libraries support data manipulation, machine learning, data visualization, and scientific computing, ensuring the project's functionality and efficiency.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/All Fields Polygons.geojson'>All Fields Polygons.geojson</a></b></td>
				<td>- The file "All Fields Polygons.geojson" is a crucial part of the project's codebase<br>- It is a GeoJSON file, a format for encoding a variety of geographic data structures<br>- This file specifically holds the geographic data for all fields in the form of polygons<br>- The main purpose of this file is to provide a structured and standardized way to store and share geographic data within the project.

In the context of the entire codebase architecture, this file serves as a data source<br>- It can be used by other parts of the project to render maps, perform spatial analysis, or any other operations that require geographic data<br>- The data in this file is referenced and utilized by other components of the project to achieve their respective functionalities<br>- The "All Fields Polygons.geojson" file is a key part of the project's data layer, providing essential geographic information that supports the functionality of the overall project.</td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- Notebooks Submodule -->
		<summary><b>Notebooks</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/Notebooks/Data_Collection_GEE.ipynb'>Data_Collection_GEE.ipynb</a></b></td>
				<td>- The file `Data_Collection_GEE.ipynb` is a Jupyter notebook that is primarily used for data collection from Google Earth Engine (GEE)<br>- It is a crucial part of the project's data pipeline, as it is responsible for gathering the necessary data that will be processed and analyzed in other parts of the project.

The notebook uses the Earth Engine Python API to authenticate and initialize a connection to a specific GEE project<br>- It then imports various libraries for data manipulation and mapping<br>- The purpose of this file is to load specific geographic data (like wheat field coordinates) and possibly perform some initial data processing.

This file is a key component in the project's data collection phase, providing the raw data that will be used throughout the rest of the project.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/Notebooks/Wheat_Yield_Data_Processing.ipynb'>Wheat_Yield_Data_Processing.ipynb</a></b></td>
				<td>- The file "Wheat_Yield_Data_Processing.ipynb" is a Jupyter notebook that is part of a larger project structure<br>- This notebook is primarily used for processing wheat yield data<br>- It imports necessary libraries such as os, pandas, and numpy, which suggests that it performs operations related to file handling, data manipulation, and numerical computations respectively<br>- The notebook likely contains a series of steps to load, clean, manipulate, and possibly visualize wheat yield data<br>- The purpose of this file is to prepare the data for further analysis or model training in the project<br>- The processed data might be used in other parts of the project for tasks such as predictive modeling, data analysis, or reporting<br>- The file's location in the "Notebooks" directory suggests that it is part of a collection of notebooks used for different data processing and analysis tasks in the project.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/Notebooks/Exploratory_Data_Analysis.ipynb'>Exploratory_Data_Analysis.ipynb</a></b></td>
				<td>- The file "Exploratory_Data_Analysis.ipynb" is a Jupyter notebook that is part of the larger project's codebase<br>- This file is primarily used for conducting exploratory data analysis (EDA) on the project's dataset<br>- In the context of the entire project, this notebook plays a crucial role in understanding the underlying patterns, relationships, and structures within the data<br>- The insights derived from this EDA process can guide the development of data models, influence the choice of data preprocessing methods, and help identify potential issues such as outliers or missing values<br>- This notebook is located in the "Notebooks" directory, indicating that it's part of a collection of similar files used for data analysis, model development, and other data science tasks<br>- The results from this notebook likely feed into other parts of the project, providing valuable context and direction for the project's overall development.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/master/Notebooks/Machine_Learning.ipynb'>Machine_Learning.ipynb</a></b></td>
				<td>- The file 'Machine_Learning.ipynb' located in the 'Notebooks' directory is a Jupyter notebook that plays a crucial role in the project's machine learning aspect<br>- It is primarily used for data analysis and modeling, likely involving the use of the pandas library for data manipulation and analysis<br>- This file is integral to the project's data science operations, contributing to the overall codebase by providing the machine learning algorithms and models that drive the project's core functionality.</td>
			</tr>
			</table>
		</blockquote>
	</details>
</details>

---
##  Getting Started

###  Prerequisites

Before getting started with Wheat_Yield_Prediction, ensure your runtime environment meets the following requirements:

- **Programming Language:** JupyterNotebook
- **Package Manager:** Pip


###  Installation

Install Wheat_Yield_Prediction using one of the following methods:

**Build from source:**

1. Clone the Wheat_Yield_Prediction repository:
```sh
❯ git clone https://github.com/dgebenicolas/Wheat_Yield_Prediction
```

2. Navigate to the project directory:
```sh
❯ cd Wheat_Yield_Prediction
```

3. Install the project dependencies:


**Using `pip`** &nbsp; [<img align="center" src="" />]()

```sh
❯ echo 'INSERT-INSTALL-COMMAND-HERE'
```




###  Usage
Run Wheat_Yield_Prediction using the following command:
**Using `pip`** &nbsp; [<img align="center" src="" />]()

```sh
❯ echo 'INSERT-RUN-COMMAND-HERE'
```


###  Testing
Run the test suite using the following command:
**Using `pip`** &nbsp; [<img align="center" src="" />]()

```sh
❯ echo 'INSERT-TEST-COMMAND-HERE'
```


---
##  Project Roadmap

- [X] **`Task 1`**: <strike>Implement feature one.</strike>
- [ ] **`Task 2`**: Implement feature two.
- [ ] **`Task 3`**: Implement feature three.

---

##  Contributing

- **💬 [Join the Discussions](https://github.com/dgebenicolas/Wheat_Yield_Prediction/discussions)**: Share your insights, provide feedback, or ask questions.
- **🐛 [Report Issues](https://github.com/dgebenicolas/Wheat_Yield_Prediction/issues)**: Submit bugs found or log feature requests for the `Wheat_Yield_Prediction` project.
- **💡 [Submit Pull Requests](https://github.com/dgebenicolas/Wheat_Yield_Prediction/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.

<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your github account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone https://github.com/dgebenicolas/Wheat_Yield_Prediction
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
   <a href="https://github.com{/dgebenicolas/Wheat_Yield_Prediction/}graphs/contributors">
      <img src="https://contrib.rocks/image?repo=dgebenicolas/Wheat_Yield_Prediction">
   </a>
</p>
</details>

---

##  License

This project is protected under the [SELECT-A-LICENSE](https://choosealicense.com/licenses) License. For more details, refer to the [LICENSE](https://choosealicense.com/licenses/) file.

---

##  Acknowledgments

- List any resources, contributors, inspiration, etc. here.

---
