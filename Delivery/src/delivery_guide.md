# CTG delivery guide

## IMPORTANT: Delivery server whitelist
You need to follow the instructions below and email us your external IP address so we
can let you through our firewall before you can download your data.

### Finding and submitting your IP:

Please note that we need to whitelist your IP address for the download to work.

For MacOS or Windows follow this link to find your IP: [www.whatismyip.com](https://www.whatismyip.com/)

Linux users can find their IP by running the following command in their terminal: `hostname -I`

Once you know your public IP email us, then we will add that IP to the whitelist.

### How to download?
*Important: Before you can download you must send us your public IP!*

You can download the data using secure copy paste (SCP) or secure file transfer protocol (SFTP). Scp is a command line utility, if you would prefer a GUI we recommend FileZilla.

In your delivery email you have received a user name already in the terminal command to download your data:  
``` scp user@lfs603.srv.lu.se:/path/to/your/data .```

In the above *user* is the username. 

If you set up a connection in filezilla you have to paste the whole username up until but not including the @ sign!

The password is given in the email as a long string of letters and numbers.

#### Using Filezilla
To download you can copy and paste the command given in the delivery email or you can set up a connection in filezilla:

[FileZilla](https://filezilla-project.org/) is a file transfer client available for multiple platforms.
To connect to our server and download our data:

1. Open the Site Manager. “File --> Site Manager” or click on the top left icon.

2. Create a “New site”

3. Set Protocol to: SFTP – SSH File Transfer Protocol

4. Type in Host: lfs603.srv.lu.se

5. Set the Port to: 22022

6. Set Logon Type to: Ask for password

7. Enter your user id that was supplied in your delivery mail.

8. Press Connect. You will now be asked for your password.

# Let us know that you downloaded the data!
If there is no storage left at our delivery server then there will be delays in our delivery routines. Therefore, it is important that you inform us when you have downloaded your data.

We keep the raw data on our secure processing HPC from the point of delivery for 1 month for sequencing only and 3 months for other projects.

# Questions?
If you have any questions please do not hesitate to contact [cglu.bioinformatics@scilifelab.se](mailto:cglu.bioinformatics@scilifelab.se), you can also reply to the delivery email! 
