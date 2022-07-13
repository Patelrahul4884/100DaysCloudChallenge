<!-- This is a template you can use for quick progress days. It removes a lot of the steps we encourage you to share in the longer template 000-DAY-ARTICLE-LONG-TEMPLATE.MD-->

# Lambda & Application Load Balancer

## Cloud Research

You can use a Lambda function to process requests from an Application Load Balancer. Elastic Load Balancing supports Lambda functions as a target for an Application Load Balancer. Use load balancer rules to route HTTP requests to a function, based on path or header values. Process the request and return an HTTP response from your Lambda function.

Elastic Load Balancing invokes your Lambda function synchronously with an event that contains the request body and metadata.

## Lambda Integration with ALB

* To expose lambda function as HTTP end point

* you can use Application load balancer or API Gateway

* Tha Lambda function must be registered in target group

* ALB to Lambda: HTTP to JSON and Lambda to ALB Conversion: JSON to HTTP

* Try enabaling multi header values in target group

If requests from a client or responses from a Lambda function contain headers with multiple values or contains the same header multiple times, or query parameters with multiple values for the same key, you can enable support for multi-value header syntax. After you enable multi-value headers, the headers and query parameters exchanged between the load balancer and the Lambda function use arrays instead of strings. If you do not enable multi-value header syntax and a header or query parameter has multiple values, the load balancer uses the last value that it receives.

The following example request has two query parameters with the same key:

http://www.example.com?&myKey=val1&myKey=val2

With the default format, the load balancer uses the last value sent by the client and sends you an event that includes query string parameters using queryStringParameters. For example:

"queryStringParameters": { "myKey": "val2"},
If you enable multi-value headers, the load balancer uses both key values sent by the client and sends you an event that includes query string parameters using multiValueQueryStringParameters. For example:

"multiValueQueryStringParameters": { "myKey": ["val1", "val2"] }

Refer following docs to learn more on Lambda with ALB and target group
[https://docs.aws.amazon.com/lambda/latest/dg/services-alb.html]
[https://docs.aws.amazon.com/elasticloadbalancing/latest/application/lambda-functions.html]

## Social Proof

[link](link)
