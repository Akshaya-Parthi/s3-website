# Deploy static website to s3 using github actions
Create a folder named website and move the project files to it.

# Create S3 bucket and configure it for static hosting:
  Visit the official documentation on how to create and set up a bucket. https://docs.aws.amazon.com/AmazonS3/latest/dev/HostingWebsiteOnS3Setup.html

# Create your Github repository:
  We need to create our github repository and configure our AWS access key and secret keys. If you don't have it, go to IAM and create your access key.
 
1.Go to https://github.com and create your repository.

2.On your github repository, go to Settings then Secrets

3.Click New Secret.

4.Enter AWS_ACCESS_KEY_ID on the Name field.

5.Enter your AWS access key on the Value field.

6.Click Add secret

Repeat 4 - 6 for the AWS_SECRET_ACCESS_KEY

# Create github actions workflow

Go to the project root directory and create a folder named .github and inside it, a folder named workflows. 

        mkdir -p .github/workflows
 
Create a file named main.yml inside the .github/workflows folder.
 
 	touch .github/workflows/main.yml

# Commit and push your changes:

	git add .
	
        git commit -m “initial commit”
  
        git push -u origin main


Go to your github repository and click on the Actions tab. From there, see all your triggered workflows and its status. 
