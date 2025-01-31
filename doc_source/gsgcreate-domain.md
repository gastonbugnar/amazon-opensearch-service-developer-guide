# Step 1: Create an OpenSearch Service domain<a name="gsgcreate-domain"></a>

**Important**  
This is a concise tutorial for configuring a *test * Amazon OpenSearch Service domain\. Do not use this process to create production domains\. For a comprehensive version of the same process, see [Creating and managing Amazon OpenSearch Service domains](createupdatedomains.md)\.

An OpenSearch Service domain is synonymous with an OpenSearch cluster\. Domains are clusters with the settings, instance types, instance counts, and storage resources that you specify\. You can create an OpenSearch Service domain by using the console, the AWS CLI, or the AWS SDKs\.

**To create an OpenSearch Service domain using the console**

1. Go to [https://aws\.amazon\.com](https://aws.amazon.com) and choose **Sign In to the Console**\.

1. Under **Analytics**, choose **Amazon OpenSearch Service**\.

1. Choose **Create a new domain**\.

1. For the deployment type, choose **Development and testing**\.

1. For **Version**, choose the latest version\.

1. Choose **Next**\.

1. Provide a name for the domain\. The examples in this tutorial use the name *movies*\.

1. Ignore the **Custom endpoint** setting\.

1. Under **Data nodes**, change the instance type to `t3.small.search` and keep the default value of three nodes\.

1. Ignore the rest of the settings for now and choose **Next**\. 

1. For simplicity in this tutorial, use a public access domain\. Under **Network configuration**, choose **Public access**\.

1. In the fine\-grained access control settings, choose **Create master user**\. Provide a user name and password\.

1. For now, ignore the **SAML authentication** and **Amazon Cognito authentication** sections\.

1. For **Access policy**, choose **Allow open access to the domain**\. In this tutorial, fine\-grained access control handles authentication, not the domain access policy\.

1. Choose **Next**\.

1. Ignore the tags option and choose **Next**\.

1. Confirm your domain configuration and choose **Confirm**\. New domains typically take 15–30 minutes to initialize, but can take longer depending on the configuration\. After your domain initializes, make note of its endpoint\.

**Next**: [Upload data to an OpenSearch Service domain for indexing](gsgupload-data.md)