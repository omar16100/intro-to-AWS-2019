# intro-to-AWS-2019

# demo : hosting a static site in AWS S3

# http://omar16100.s3-website-ap-southeast-1.amazonaws.com/

# Steps 

1 Create an AWS account

2 Search for 'S3' in the management console

3 Click on the S3 console

4 Create a bucket

5 Navigate to Permissions

6 Copy and paste "{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::BUCKET/*"
    }
  ]
}
"

Replace BUCKET with your own bucket name.

7 Click 'Save'

8 Navigate to 'Properties'

9 Enable 'Static Website Hosting'

10 Upload your files for the static website (clone/copy the files oof this directory and upload for testing purposes)




references

 - https://github.com/n5hossai/naymulhulk.github.io
 
 - https://www.qwiklabs.com/focuses/400?catalog_rank=%7B%22rank%22%3A1%2C%22num_filters%22%3A0%2C%22has_search%22%3Atrue%7D&parent=catalog&search_id=3761935

