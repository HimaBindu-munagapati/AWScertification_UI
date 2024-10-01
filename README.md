Certainly! Here's a reformatted and more readable version of your README file:

---

# Create and Host a Static Website using Amazon S3

## Step 1: Create a Bucket in Amazon S3
1. **Navigate to S3**  
   - Go to the **AWS Management Console** and search for `S3`.
   
2. **Create a Bucket**
   - Choose **Create bucket**.
   - **AWS Region**: Select the region closest to you.
   - **Bucket name**: Enter `nextwork-website-project-name`.  
     > Replace `project-name` with your name (e.g., `nextwork-website-johndoe`).  
     💡 Note: S3 bucket names must be globally unique. Once created, no other AWS account in the world can use your bucket's name unless you delete it.

3. **Configure Object Ownership and ACLs**
   - For **Object Ownership**, select **ACLs enabled**.
   - Choose **Bucket owner preferred**.

4. **Set Block Public Access Settings**
   - Clear the check box for **Block all public access**.
   - A yellow warning banner will pop up:  
     > This banner tells you that the bucket and its objects might become public if you untick the checkbox. This is what we want to host a public website!
   - Check the box that says:  
     > “I acknowledge that the current settings might result in this bucket and the objects within becoming public.”

5. **Enable Bucket Versioning**
   - For **Bucket Versioning**, choose **Enable**.

6. **Create the Bucket**
   - Choose **Create bucket**.

## Step 2: Upload Website Content to Your Bucket
1. **Select Your Bucket**
   - Go to the **Amazon S3 console**.
   - Choose the name of your new bucket.

2. **Upload Website Files**
   - Unzip the zip file containing your website's files.
   - On your bucket page, go to the **Objects** tab.
   - Choose **Upload**.
   - Choose **Add files**, then select `index.html`.
   - Choose **Add folder**, then select the **un-zipped folder** (not the zip file itself).
   - If a popup appears, confirm that all files in the folder will be uploaded.
   - Choose **Upload**.
   
3. **Complete Upload**
   - Wait for the upload to finish.
   - Once you see the green **Upload succeeded** banner, choose **Close**.

## Step 3: Configure Static Website Hosting on Amazon S3
1. **Go to the Properties Tab**
   - Make sure you're back on your bucket's main page.
   - Choose the **Properties** tab.

2. **Enable Static Website Hosting**
   - Scroll to the **Static website hosting** panel.
   - Choose **Edit**.
   - Configure the following settings:
     - **Static web hosting**: Choose **Enable**.
     - **Hosting type**: Select **Host a static website**.
     - **Index document**: Enter `index.html`.
   - Choose **Save changes**.

3. **View Your Website**
   - Go back to the **Static website hosting** panel.
   - Under **Bucket website endpoint**, click on the URL.

4. **Make the Bucket Public**
   - If you see an error (e.g., `403 Forbidden`), go back to the **Permissions** tab.
   - Choose **Make public**.
   - Once the green banner pops up, choose **Close**.

5. **Verify Your Website**
   - Return to the web browser tab with the `403 Forbidden` error.
   - Refresh the tab, and your website should load successfully!

---

This version is structured and highlights the key steps clearly, making it easier to follow and implement. Let me know if you'd like to add anything else!
