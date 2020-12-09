# Amazon Web Services Free Tier
Amazon Web Services (AWS) has three types of free offers available depending on the product that you choose: free tier, 12 months free, and trials. The details of each free offer can be found here: https://aws.amazon.com/free/free-tier/.

All activities in the Big Data unit will use free tier services. However, it is still possible to [incur charges](https://aws.amazon.com/getting-started/hands-on/control-your-costs-free-tier-budgets/) while using the free tier service. Therefore, before you sign up and use any AWS Free Tier service, make sure you review all the services and resources covered under [AWS Free Tier](https://aws.amazon.com/free/). AWS provides additional information on how to avoid free tier charges [here](https://aws.amazon.com/getting-started/hands-on/control-your-costs-free-tier-budgets/).


# Cloud Storage on S3

* Go to **console.aws.amazon.com** and select **S3** under **Storage**.

![s3 console](Images/s3_console.png)

* Click **Create bucket**.

![click create](Images/create_bucket.png)

* Create a bucket name and choose the region.

* **Note:** The bucket name must be unique across all existing bucket names in Amazon S3. Buckets cannot be renamed or created inside of another bucket.

* Leave the region as the default, e.g. `US East (N. Virginia)`. Changing the region will change the object URL used in all examples today.

![Images/s301.png](Images/s301.png)

* Most of the options on the **Configure Options** page can be left as default values.

* **Tags** are user-defined key-value pairs of information that can help keep track of buckets.

* Click **Next**.

![Images/s302.png](Images/s302.png)

* The **Set Permissions** page is where we grant others permission to access buckets.

  * A number of [security breaches](https://securityboulevard.com/2018/01/leaky-buckets-10-worst-amazon-s3-breaches/) were caused by unsecured S3 buckets.
  
  * Public access is denied by default.

  * Leave the boxes checked and click **Next**.

    ![Images/s303.png](Images/s303.png)

* The **Review** page is a summary of the bucket configurations. Click **Create bucket**. The bucket name now appears in the S3 console.

    ![Images/s304.png](Images/s304.png)

    ![Images/s305.png](Images/s305.png)

* We'll now upload an image file to the newly created bucket. Click the bucket name and then click **Upload**.

  * A file can be dragged to the screen.

  * Click **Upload**.

    ![Images/s315.png](Images/s315.png)

    ![Images/s316.png](Images/s316.png)

  * Click the filename.

    ![Images/s317.png](Images/s317.png)

  * Clicking the link leads to an error message! Why?

    ![Images/s308.png](Images/s308.png)

    ![Images/s309.png](Images/s309.png)

  * By default, the permission for the file denies access to everyone, so it needs to be changed.

  * Navigate back to the dashboard by clicking **Amazon S3** on the top left.

    ![Images/s3_dashboard](Images/s3_dashboard.png)

  * Check the box next to your bucket and click **Edit public access settings**.

    ![Images/edit_public.png](Images/edit_public.png)

  * Make sure all boxes are unchecked on the next screen. Even though these were checked in the initial setup, they will not be now.

    ![Images/bucket_public.png](Images/bucket_policy.png)

  * Click **Save**. Then type **confirm** and click **Confirm**.

    ![Images/confirm_policy.png](Images/confirm_policy.png)

  * Next, navigate back into your bucket and check the box next to the image. Click the **Actions** box on the top and select **Make public**.

    ![Images/bucket_public.png](Images/bucket_public.png)

  * Now the image will be displayed when you click on the link.

* You can explore various settings at the bucket level and the file level. Use the tabs at the bucket level to explore the available settings, such as tags:

  ![Images/s306.png](Images/s306.png)

* **Note:** You can remove public access anytime by repeating the steps above and checking all the boxes in **Edit public access settings**.
