# DVC Bitcoin SNA

This project partially re-implements the Github SNA Colab Notebook using DVC and pipelines. Since the initial Colab Notebook was really extensive, only few sections have been reimplemented here for the purpose of this exercise.

In particular, the following sections have been ported to DVC pipelines

- Data Intialization
  
- Prepare

      	                             +-------------------------------------+                   
                                           | data/soc-sign-bitcoinalpha.csv.dvc |                   
                                           +-------------------------------------+                   
                                                        *                             
                                                        *                              
                                                        *                             
                  	                              +---------+                        
                  	                              | prepare |                        
                  	                              +---------+      

Input data are located in the folder data/soc-sign-bitcoinalpha.csv, while output data are also located in the folder data. We will get output as Network Graph.


# Download

Clone the project.

In terminal, copy the below the link to clone the project code in your local directory.

    git clone https://github.com/Prem948/DVC-Bitcoin-SA.git

# Setup

Python 3 is required, so please check it if you have installed it on your system. This project has been developed with Python 3.9.

By using terminal, open the directory of the clone project to run.

    cd DVC-Bitcoin-SNA
      
# Install the required python packages

    pip install -r src/requirements.txt
    
# Run

Using the terminal, execute the following command and see the Social Network Ego Graph:

    dvc repro
    
To visualize the pipeline graph run the following command

    dvc dag
    
# Examples

You can save the Ego Graph in your local directory by clicking save in that Output Graph.
