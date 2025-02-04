--- 
hide_table_of_contents: true
hide_title: true
---


### Prerequisites

- An [Amazon Web Services](https://aws.amazon.com) account.

---

**Perform the following steps to configure your Amazon S3 Sink.**

### Step 1: Create an AWS User

1. Log in to the AWS [Management Console](https://aws.amazon.com) using your root account credentials.
2. Navigate to the [IAM](https://console.aws.amazon.com/iam/) service by searching for `IAM` and clicking the IAM service.
   ![](images/1.png)
3. Click on the **Users tab** in the left navigation menu, and then click the **Add user** button.
   ![](images/2.png)
4. Write a name for your user and click **next**.
   ![img.png](images/3.png)
5. Select **Attach policy directly**, and **Create policy**.
   ![](images/4.png)
6. Search for s3 and select it.
   ![](images/5.png)
7. Next, search for the following policy.
    - "PutObject",
    - "GetObject",
    - "GetObjectVersion",
    - "DeleteObject",
    - "DeleteObjectVersion"
      ![](images/6.png)
8. Press **Next** and proceed to the next page.
   ![](images/7.png)
9. Name your policy and click **Create policy**.
   ![](images/8.png)
10. Return back to your previous `TAB`.
    ![img.png](images/8.1.png)
11. Search for your custom policy and add it to your account, and press **Next**.
    ![img.png](images/9.png)
12. Review and press **Create user**.
    ![img.png](images/10.png)

---

### Step 2: Get your Access key and Secret access key

1. Now click on the user you just created.
   ![img.png](images/11.png)
2. Under **Security credentials**, scroll down the page to `Access Key`, and Click **Create access key**.
   ![](images/12.png)
3. Select Command line interface CLI, and press **Next**.
   ![img.png](images/13.png)
4. Click **Create access key**.
   ![img.png](images/14.png)
5. Save your `Access key` and `Secret access key` safely.
   ![](images/15.png)

---

### Step 3: Amazon S3 Connection Settings

**To set up S3 Sink in Vanus Connect:**

1. Enter your `Access Key` and `Secret access Key` in Vanus Connect from the previous steps.
2. Now let's go back to Amazon Web Services under the [Amazon S3 service](https://s3.console.aws.amazon.com).
3. At this point, you can either **create a new bucket** or **select an existing** bucket.
4. Once you've chosen or created a bucket, keep in mind your bucket name and region.
![img.png](images/16.png)
5. Write your `bucket name` and select your `region` in Vanus Connect.
![](images/17.png)
6. Select the interval time of upload; `HOURLY` or `DAILY`
7. Click **Next** to continue.

---

Learn more about Vanus and Vanus Connect in our [documentation](https://docs.vanus.ai).
