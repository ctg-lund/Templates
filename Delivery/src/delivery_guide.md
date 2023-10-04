# CTG delivery guide

## IMPORTANT: Delivery server whitelist
You need to follow the instructions below and email us your external IP address so we
can let you through our firewall before you can download your data!

### Finding and submitting your IP:

Please note that we need to whitelist your IP address for the download to work.

Follow one of these guides depending on you OS

MacOS or Windows:

[IP adress for windows and mac](https://www.whatismyip.com/)

Linux:

Write ```hostname -I``` in the terminal.



Once you know your public IP send us an email and we will add that IP to the whitelist!

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

*[FileZilla](https://filezilla-project.org/) is a file transfer client available for multiple platforms .*
*To connect to our server and download our data:*
1. Open the Site Manager. “File --> Site Manager” or click on the top left icon.
2. Create a “New site”
3. Set Protocol to: SFTP – SSH File Transfer Protocol
4. Type in Host: lfs603.srv.lu.se
5. Set the Port to: 22022
6. Set Logon Type to: Ask for password
7. Enter your user id that was supplied in your delivery mail.
8. Press Connect. You will now be asked for your password.


# Let us know that you downloaded the data!
Genomic data is very large and CTG is steadily growing at a fast pace, because of this we ask that you let us know when we no longer need to host your data on our delivery server. This way we can free up space and avoid delays in our delivery routines!

In case you are worried about losing the raw data, we always keep the raw data on our secure processing HPC for the time specified when you make your request. This is at the moment 1 month for sequencing only and 3 months for everything else. The delivery server is a separate system that contains all the result files! 

# Questions?

If you have any questions please do not hesitate to contact [email](mailto:cglu.bioinformatics@scilifelab.se), you can also reply to the delivery email! 
