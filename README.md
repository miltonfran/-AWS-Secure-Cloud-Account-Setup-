<h1>AWS Secure Cloud Account Setup</h1>
 
<h1></h1>

<h2>Description</h2>
This is a step-by-step guide to creating and securing an Amazon Web Services (AWS) free-tier account with professional-grade security practices. The tutorial is designed for individuals, particularly those in DevOps and cloud computing, who want to create a robust and secure AWS cloud environment.
<br />
<h2>Utilities and Tools</h2>

- <b>Authentication Tools
Google Authenticator (for Multi-Factor Authentication)
Password managers (recommended)</b> 

- <b>Web Browsers
Any modern web browser (Chrome, Firefox, Brave, etc.)</b> 
- <b>Cloud Platform
Amazon Web Services (AWS)
Free Tier Account
Regions (specifically North Virginia)</b>

- <b>AWS Services Used
IAM (Identity and Access Management)
CloudWatch
EC2 (mentioned)
Certificate Manager (ACM)
Simple Notification Service (SNS) </b>


<h2>Environments Used </h2>

- </b> Operating System: Ubuntu Linux (running on an AWS EC2 instance)</b>
- </b> Cloud Platform: Amazon Web Services (AWS EC2)</b>
-</b> Network Configuration: Security groups to enable HTTP (port 80) and SSH (port 22) traffic</b>

<h2>Program walk-through:</h2>

<p align="center">
 Create Free AWS Account/: Open AWS free tier website
Click "Create a Free Account"
Enter email address
Verify email with code
Create a strong root user password<br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733959176/Screenshot_2024-12-10_214142_xqrmge.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733959359/Screenshot_2024-12-10_214209_pjcz0q.png"/>
<br />
<br />
 
Complete Account Registration Fill in personal account details Add credit/debit card for verification Verify phone number Select basic support plan Complete sign-up: <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733959447/Screenshot_2024-12-10_214222_cnprml.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733968006/Screenshot_2024-12-10_214237_xdsazz.png"/>
<br />
<br />

Verify Account Activation Log into AWS Management Console Check EC2 service Ensure the account is active with zero instances: <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733968225/Screenshot_2024-12-10_214504_u82ys8.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733968339/Screenshot_2024-12-10_214524_wyxmpp.png"/>
<br />
<br />
Set Up Multi-Factor Authentication for Root User Go to IAM service Enable MFA for root user Install Google Authenticator app Scan QR code Set up MFA authentication: <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733968426/Screenshot_2024-12-10_214540_p3nfic.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733968496/Screenshot_2024-12-10_214607_pngwri.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733974683/Screenshot_2024-12-10_214626_l4tltf.png"/>
<br />
<br />
Create IAM User Go to IAM Users Create a new user (e.g., IT Admin) Assign Administrator Access Enable Console Access Set auto-generated password Require password reset at first login Set up MFA for IAM user: <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733975135/Screenshot_2024-12-10_215426_wuafol.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733975445/Screenshot_2024-12-10_215506_xfkez5.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733975998/Screenshot_2024-12-10_215920_gdqbtg.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733976554/Screenshot_2024-12-10_215959_m8x2wk.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733976893/Screenshot_2024-12-10_220029_aq2bfr.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733977162/Screenshot_2024-12-10_220348_qtzhnq.png"/>
<br />
<br />
Configure Billing Preferences Go to Billing Dashboard Enable invoice delivery preferences Enable AWS Free Tier alerts Enable CloudWatch billing alerts:  <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733977892/Screenshot_2024-12-10_220415_tvwi8x.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733977954/Screenshot_2024-12-10_221023_q1amnl.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733978129/Screenshot_2024-12-10_221054_msmx8p.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733978197/Screenshot_2024-12-10_221444_u9vciy.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733977110/Screenshot_2024-12-10_220107_rkkzve.png"/>
<br />
<br />

Create Billing Alarm Go to CloudWatch Select North Virginia region Create billing alarm Set threshold (e.g., $5) Create SNS topic for notifications Confirm email subscription  <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733979563/Screenshot_2024-12-10_221533_nuxzxd.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733979702/Screenshot_2024-12-10_221548_xujywu.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733979902/Screenshot_2024-12-10_221656_h8haeo.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733982685/Screenshot_2024-12-10_224157_ymw9ka.png"/>
<br />
<br />

Create SSL Certificate (Optional) Go to AWS Certificate Manager Request public certificate Use DNS validation Add CNAME record with domain registrar Wait for certificate validation  <br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733983301/Screenshot_2024-12-10_224744_x6rbbm.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733983429/Screenshot_2024-12-11_003430_vazo3i.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733983463/Screenshot_2024-12-11_003738_lupnc8.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733983575/Screenshot_2024-12-11_003752_iuci0g.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733983627/Screenshot_2024-12-11_151910_qq69uo.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733984321/Screenshot_2024-12-11_151921_kklbpy.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733984570/Screenshot_2024-12-11_151940_wzpbvh.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733984631/Screenshot_2024-12-11_151952_aej0tx.png"/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733984745/Screenshot_2024-12-11_152308_egjjz7.png"/>
<br />
<br />


Create Account Alias Go to IAM Dashboard Create a custom account sign-in URL Save custom alias  <br/>


Log In with IAM User, Use custom sign-in URL Log in with IAM user credentials Complete first-time login Reset password<br/>
<img src="https://res.cloudinary.com/dk3bkl3ji/image/upload/v1733984966/Screenshot_2024-12-11_152518_ntxd5g.png"/>







