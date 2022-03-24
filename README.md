# What Is This?
With this repo, you can save your website visitors number on AWS Dynomodb and you can easily expose as api with AWS Lambda Function. İf you want to add visitor number to your website you should use javascript. In this repo, you will learn your website visitors. 




## Creating Services
First you should create an AWS account. After that you need to create a table named VisitorCount from DynamoDB and partition key must be id(String). 

![image](https://user-images.githubusercontent.com/54737933/159992711-9941e470-5f6b-47d8-b023-465cdb473c89.png)


Than you should edit Item editor like this. After that you should create a Lambda and API Gateway.




## Lambda Function
> This repo does not explain AWS setup. If you are having problems about setting up AWS services. Please review the required documents. 

First we are going to write a Lambda Function. Then you will install the `lambda_function.py`. Import or copy everything like this.

![image](https://user-images.githubusercontent.com/54737933/159993039-5b51c5e4-d3fa-4b9f-9c1b-3a35b7190cad.png)


After that create a Get Method in API Gateway. Connect the API Gateway with DynamoDB. After that you should Deploy API and Enable CORS.

![image](https://user-images.githubusercontent.com/54737933/159994916-e9d9098a-74c0-4a46-b309-e740fe090555.png)

If you're making the right adjustments, you need this building.




## Usage of HTML and Javascript
In this part, we should add javascript command in our website code. You should Write this command inside the HTML code.

```html
<script>
    		fetch('https://xxxxxxxxxx.execute-api.eu-west-1.amazonaws.com/beta') // You should change the link.
      		.then(response => response.json())
      		.then((data) => {
        	document.getElementById('visitor_counter').innerText = data.Count
      		})
</script>
```

With this command now you can call the value. 

If you want to write this value to your website, you should add this command to your HTML code. 
```<span id="visitor_counter" />```

After all of that, you can use visitor counter in your website.


You can see an example in [here](https://kuzeyardabulut.com/).
