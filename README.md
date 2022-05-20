# Module-10-Challenge - Crypto Clustering
This application takes advantage of unsupervised learning aspect of Machine Learning to cluster the crypto performance data over past specified periods.

The Starter Code was provided along with the historical crypto data for prior periods.

---

## User Story
Your company wants to present a crypto portfolio to the upper management that will include the performance of the varuous cryptos in a cluster format in addition to the volatility and returns information. 

---

## Acceptance Criteria  
The application must meet the following acceptance criteria:  

* Import the Data from a csv file (provided in the starter code)  
* Prepare the Data using StandardScaler (provided in the starter code)  
* Find the Best Value for k Using the Original Data  
* Cluster Cryptocurrencies with K-means Using the Original Data  
* Optimize Clusters with Principal Component Analysis  
* Find the Best Value for k Using the PCA Data  
* Cluster the Cryptocurrencies with K-means Using the PCA Data  
* Visualize and Compare the Results  
  
---

## The Application  

The application follows these stages: 
    
### Import and Prepare the Data provided in the Starter Code       
* Extract the crypto data from the csv file and standardize it using StandardScaler so the resulting scaled dataframe could be used by the application.  

### Find the best value of k using the Original Data  
* Use Elbow method to find the best k value  

### Cluster Cryptocurrencies using KMeans Algorithm using Original Data  
* Use KMeans algorithm to find the clusters using the best k found above  
* Display the clusters using hvplot scatter plot  

### Optimize Clusters with Prinicipal Component Analysis (PCA)    
* Using PCA create a model with 3 components 
* Display the **explained variance**  
* Create the PCA dataframe. 

### Find the best value of k using PCA Data  
* Use the Elbow method to find the best value for k  

### Cluster Cryptocurrencies using KMeans Algorithm using PCA Data  
* Use KMeans algorithm to find the clusters using the best k found above    
* Display the clusters using hvplot scatter plot   

### Visualize and Compare the Results  
* Vislualize and compare the Elbow plots with Original Data against the PCA Data  
* Visualize and compare the scatter plots with Original Data against the PCA Data  
---

## Technologies
The application is developed using:  
* Language: Python 3.7,   
* Packages/Libraries: Pandas, hvplot.pandas; KMeans, PCA, and StandardScaler from sklearn library
* Development Environment: VS Code and Terminal, Anaconda 2.1.1 with conda 4.11.0, Jupyterlab 3.2.9  
* OS: Mac OS 12.1

---
## Installation Guide
Following are the instructions to install the application from its Github respository.  

### Clone the application code from Github as follows:
copy the URL link of the application from its Github repository      
open the Terminal window and clone as follows:  

    1. %cd to_your_preferred_directory_where_you want_to_store_this_application  
    
    2. %git clone URL_link_that_was_copied_in_step_1_above   
    
    3. %ls     
        Module-10-Challenge    
        
    4. %cd Module-10-Challenge     

At this point you will have the the entire application files in the current directory as follows:

    * README.md                   (this file that you are reading)  
    * crypto_investments.ipynb          (the application jupter lab notebook)  
    * Resources                      (Folder with crypto csv file  
        - crypto_market_data.csv     (Crypto data file in csv format)

---

## Usage
The following details the instructions on how to run the application.  

### Setup the environment to run the application
Setup the environment using conda as follows:

    5. %conda create dev -python=3.7 anaconda  
    
    6. %conda activate dev  
    
    7. %jupyter lab  

---

### Run the Application
THIS ASSUMES FAMILIARITY WITH JUPYTER LAB. If not, then [click here for information on Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/).  

After step 7 above, this will take you to the jupyter lab window, where you can open the application notebook **crypto_investments.ipynb** and run the application.  

**NOTE**:
>Your shell prompt will look something like __(dev) ashokpandey@Ashoks-MBP dir%__ ,  with:  
    - '(dev)' indicating the activated 'dev' environment,   
    - ' ashokpandey@Ashoks-MBP ' will be different for you as per your environment, and   
    - 'dir' directory is where the application is located.  
    - '%' sign is the shell prompt - it may be a dollar sign in your implementation 

---

## Contributors
Ashok Pandey - ashok.pragati@gmail.com   
www.linkedin.com/in/ashok-pandey-a7201237

---

## License
The source code is the property of the developer. The users can copy and use the code freely but the developer is not responsible for any liability arising out of the code and its derivatives.

---