Create a bucket in Amazon S3

In the AWS Management Console, Search for S3.
Choose: Create bucket
AWS Region: select the Region closest to you.
For Bucket name, enter nextwork-website-project-name, Make sure to replace name with your name.
💡 An S3 bucket name is globally unique, and all AWS accounts share the namespace. After you create a bucket, no other AWS account in the entire world can use your bucket's name unless you delete the bucket.
For Object Ownership choose ACLs enabled
Step 1: Make sure ACLs are enabled! Don't get tripped up by this common error.
Choose Bucket owner preferred
For Block Public Access settings for this bucket clear the check box for Block all public access
💡 A yellow banner has popped up! This banner is telling us that the bucket and its objects might become public if we untick the checkbox. This is what we want to host a public website!
Check the box that says “I acknowledge that the current settings might result in this bucket and the objects within becoming public.”
For Bucket Versioning choose Enable
Choose Create bucket
Upload website content to your bucket
Time to get your website's files in your bucket!
In the section, choose the name of your new bucket.
Upload these files into your bucket (right click on each link, and select ):
Unzip the zip file you've downloaded.
Return to the Amazon S3 console with your bucket page open. Choose the Objects tabs.
Choose Upload
Choose Add files
Choose index.html
Choose Add folder
Choose the unzipped folder - NOT the zip file itself!
You might get a popup that tells you that all files in that folder will be uploaded.
Choose Upload
S3 will get to work right away!
Your files should upload in a few minutes! Choose Close, when you see the green Upload succeeded banner.
🌐 Step #3
Configure a static website on Amazon S3
Now let's set up the bucket for static website hosting!

Make sure you're back in your bucket's page. If you're not sure, choose buckets, on the left hand side navigation bar, and then choose the bucket you created for this project.
Choose the Properties tab.
Scroll allllllllll the way down to the Static website hosting panel.
Choose Edit
Configure the following settings:
Static web hosting: Choose Enable 
Hosting type: Choose Host a static website
Index document: Enter index.html
Choose Save changes
In the Static website hosting panel under bucket website endpoint, click on the URL.
An error! 👀
Choose Make public.
Once the green banner pops up, choose Close
Return to the web browser tab that has the 403 Forbidden message.
Refresh the tab.
