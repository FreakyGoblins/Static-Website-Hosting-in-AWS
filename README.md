# Static-Website-Hosting-in-AWS (Using CORS)
[Note: CORS is a way for client web applications that are loaded in one domain to interact with resources in different domain)
# Static-Website-Hosting
# Creating a static website in 5 minutes using S3 on AWS
# Steps:
# 1. First create 2 buckets in s3 and upload 2 files namely index.html and fetch.html in two differnt buckets .
# 2. Here index.html is a html file where fetch.html is linked here in index.html using fetch command in index.html .
# 3. Now here is where we use CORS thus we can connnect both index.html and fetch.html from differnt bucket .
# 4. After creating 2 buckets and uploading index.html in first bucket and fetch.html in second bucket .Go to the bucket and in permission >> block public access >> unblock all .Do it for both the bucket.
# 5. In bucket >>permission >>Enable ACL >>Enable everyone public access .Then scroll down and enable Static hosting .Do this for both the Bucket .
# 6. Same go to both files we uploaded, enable ACL and give public access to it.
# 7. In this case fetch.html is the html file its attached in index.html coding so we have to enable CORS in for fetch.html. 
# 8. Go to second bucket where fetch.html is there , Go to permissiom >>enable CORS by editing some comtent in the box.CORS >>Learn more >>Using the S3 console >>CORS Configuration >>copy Example 1 and paste it in CORS box in bucket 2 .There in Allowed Origin just remove if any origin is there and just paste the URL of index.html .
# 9. Now paste the index.html URL in the browser we will get the both index.html and fetch.html in one URL .This is the use of CORS.

# Note : In index.htnl code there will be a line where we need to paste the fetch.html URL there .Dont forget to add that inside single qoutes.

# I will share the sample code of index.html and fetch.html in a seperate .md file you can see that there.


# Output

# fetch.html

![Screenshot-_46_](https://github.com/FreakyGoblins/Static-Website-Hosting-in-AWS/assets/143277720/7525bd2c-dbdf-46fa-a39c-4dc61167e860)


# index.html

![Screenshot-_47_](https://github.com/FreakyGoblins/Static-Website-Hosting-in-AWS/assets/143277720/27a72479-59d3-428a-bf9d-5c0a4acbb5b6)

