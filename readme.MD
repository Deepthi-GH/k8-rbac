````
eksctl utils associate-iam-oidc-provider --cluster roboshop-dev --approve
````
eksctl create iamserviceaccount --cluster roboshop-dev --name secret-reader --namespace roboshop --attach-policy-arn arn:aws:iam::485658242739:policy/RoboshopMySQLSecretReader --approve
