--- 
hide_table_of_contents: true
hide_title: true
---

### Prerequisites

- Have an ElasticSearch cluster. 

---

**Perform the following steps to configure your ElasticSearch Sink.**

### Step 1: Setup an Elasticsearch cluster 

1. Go to the [Elasticsearch](https://www.elastic.co/) official website and sign up for an account.  
![](images/1.png)   


2. Input your name and company, select your interest and reason for using Elastic search, and click next.  
![](images/2.png)   


3. Create your deployment. A deployment includes Elasticsearch, Kibana, and other elastic stack features
![](images/3.png)    

- Name your deployment.  

- Choose the cloud provider you want to make use of.  

- Select your region.  

- You can leave the other settings on default or customize your settings further, depending on your use case. We left them on default because the default settings are sufficient for our use case.  

- Click on **create deployment** to finish creating your deployment.  


4. Download your deployment credentials, you will need them to log in to your endpoint, and they will also be needed for your Vanus connection.  
![](images/4.png)   


5. Wait for the creation of your deployment to be completed.     


6. Your deployment has been successfully created, now click **continue**.
![](images/5.png)   


#### Getting your server endpoint

1. Click on the **settings** icon on the right side of your deployment.  
![](images/6.png)   


2. Copy your Elasticsearch endpoint.  
![](images/7.png)   


3. Paste the copied endpoint in your browser, fill in the credentials you downloaded while creating your deployment and click on sign in. 
![](images/8.png)   

![](images/9.png)   


#### Creating an Index

1. Click on API Console  
![](images/10.png)   

2. Select the **PUT** option, write the name of your index, and click submit. For this tutorial, we named our index **"my_index".** 
![](images/11.png)   

    
![](images/11.1.png) 

3. Add a backslash and your index name to your endpoint to see the content of your index. 
![](images/12.png)   

---

### Step 2: ElasticSearch Connection Settings

1. Provide the following credentials
   - Server Endpoint: The endpoint of your ElasticSearch cluster.  
   - Index: The name of the index you created.  
   - Username: The username you downloaded during the creation of your deployment.   
   - Password: The password you downloaded during the creation of your deployment.  
    
2. Click `Next` and finish the configurations.

---

Learn more about Vanus and Vanus Connect in our [documentation](https://docs.vanus.ai).
