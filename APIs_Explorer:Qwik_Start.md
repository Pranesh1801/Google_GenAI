## Run in cloudshell

```cmd
export PROJECT_ID=$(gcloud config get-value project)
gsutil mb -p $PROJECT_ID -c regional -l us-central1 gs://$PROJECT_ID-bucket
curl -O https://github.com/siddharth7000/practice/blob/main/sign.jpg
mv sign.jpg demo-image.jpg
gsutil cp demo-image.jpg gs://$PROJECT_ID-bucket/demo-image.jpg
gsutil acl ch -u allUsers:R gs://$PROJECT_ID-bucket/demo-image.jpg
```

Open the lab "APIs Explorer: Qwik Start"
Sign in to your account in the incognito window with the account details provided after start lab.
open the cloud console from the terminal icon from the top right side of the page.
paste the above code.
click enter and authorise
go back to the course and click check my progress.

