# Configuring MFA in AWS IAM

![AWS MFA](https://imgur.com/qqU87hA.jpg)


## Introduction

This project demonstrates the step-by-step process of configuring Multi-Factor Authentication (MFA) within AWS IAM. Implementing MFA enhances the security of user accounts by requiring an additional verification step during the login process.

### Component used:

- Amazon Web Service (AWS)
  - AWS IAM
- Authy (authenticator application)

## Select User for MFA Setup 

In the AWS IAM console, navigate to the Users menu and select the user for whom you want to enable MFA. For this project, we’ll use user 'Q1'. 

![---](https://imgur.com/k2YK0UB.jpg) 

## Enable Console Access 
If console access is disabled, enable it by creating a password for the user. Go to the Security credentials tab and select 'Enable console access'.
![---](https://imgur.com/ayTkTUJ.jpg) 

![---](https://imgur.com/p2rasDh.jpg) 

Create a password and save it for the user account.

![---](https://imgur.com/0A8Antn.jpg) 

Now the console has been enabled.

![---](https://imgur.com/OZRSSFN.jpg) 

## Assign MFA Device 

Once console access is enabled, proceed to 'Assign MFA device.' Create a device name and select your preferred option. For this project, we’ll use the Authenticator App option. 

![---](https://imgur.com/sLKGwJ4.jpg) 

![---](https://imgur.com/ASPdKvw.jpg) 

Select Show QR code.

![---](https://imgur.com/57BGis8.jpg) 

## Configure Authenticator App 

On your mobile authenticator application (e.g., Authy), scan the QR code provided by AWS. Enter two consecutive MFA codes into the provided fields. 

![---](https://imgur.com/BATvBIT.jpg) 

We will now scan the QR code provided on AWS' Assign MFA device screen followed by entering two consecutive MFA codes in the provided fields.

![---](https://imgur.com/jK49Ldc.jpg)  

![---](https://imgur.com/sf6wtF6.jpg) 

On the authenticator application, we will provide a nickname for the newly added account. 

![---](https://imgur.com/v8ftMDL.jpg)  

Now we can see that the Q1 account has been successfully added.

![---](https://imgur.com/nnExda9.jpg)  

## Test MFA Implementation 

We have a confirmation suggesting the MFA implementation process was successful.

![---](https://imgur.com/QbkSSTG.jpg)  

![---](https://imgur.com/3ScrvKH.jpg) 

Confirm the MFA configuration by signing out of the admin account and signing into the user account with the new MFA setup.

![---](https://imgur.com/IBWbNOu.jpg) 

Enter the current MFA code from the authenticator application to complete the login process. If successful, you’ve enabled MFA for your user account in AWS. 

![---](https://imgur.com/IhlLwDq.jpg) 

If you were able to sign in then you have successfully enabled MFA for your user account in AWS! 

![---](https://imgur.com/EnibhEZ.jpg) 

## Conclusion
In this project, we successfully configured Multi-Factor Authentication (MFA) for a user in AWS IAM, enhancing account security and ensuring an additional layer of protection.

## fin
