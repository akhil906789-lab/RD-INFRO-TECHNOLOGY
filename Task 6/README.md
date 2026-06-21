# Task 6: Set Up a Serverless Function

## Objective

Deploy code using Function-as-a-Service (FaaS) with AWS Lambda and expose it using API Gateway.

---

## Tools Used

* AWS Lambda
* API Gateway
* Python

---

## Files

* lambda_function.py
* README.md

---

## Lambda Function Code

```python
def lambda_handler(event, context):
    return {
        'statusCode': 200,
        'body': 'Hello from AWS Lambda! RD INFRO TECHNOLOGY Internship'
    }
```

---

## Procedure

1. Open AWS Lambda Console.
2. Create a function named `Task6-Lambda`.
3. Select Python runtime.
4. Write the Lambda function code.
5. Deploy the function.
6. Create a test event named `Task6Test`.
7. Execute the function and verify the response.
8. Add an API Gateway trigger.
9. Create an HTTP API endpoint.
10. Access the endpoint URL through a web browser.

---

## Output

```
Hello from AWS Lambda! RD INFRO TECHNOLOGY Internship
```

---

## Screenshots

### Lambda Function Code

![Lambda Code](Lambda_Code.png)

### Lambda Test Output

![Lambda Test Output](Lambda_Test_Output.png)

### API Gateway Trigger

![API Gateway Trigger](API_Gateway_Trigger.png)

### Browser Output

![Browser Output](Browser_Output.png)

---

## Result

Successfully created and deployed a serverless function using AWS Lambda and integrated it with API Gateway. The function was tested successfully and invoked through a browser using the generated API endpoint.
