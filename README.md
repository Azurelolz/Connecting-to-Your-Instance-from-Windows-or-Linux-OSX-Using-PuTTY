# Connecting-to-Your-Instance-from-Windows-or-Linux-OSX-Using-PuTTY
Connecting to Your Instance from Windows or Linux/OSX Using PuTTY.

### Connect to your instance (Linux/OSX only)

>Note: This section is for Linux and Mac OSX users only. If you are running Windows but have not yet connected to your instance, go back to previous step. If you have already connected to your instance, skip ahead to next step.

1. To connect to your EC2 instance, run the following commands in Terminal:
```
chmod 400  <path and name of pem>
ssh –i <path and name of pem> ec2-user@<public IP>
```

* For **path and name of pem**, substitute the path/filename to the .pem file you downloaded.
* For **public IP**, substitute the public IP address for your **Web Server** instance which you copied into a text editor earlier in the lab.


### Connect to your instance (Windows only)

1. Start PuTTYgen.exe, click **Load**. By default, PuTTYgen display only files with the extension .ppk. to locate your .pem file, select the option to display files of all types.

![4.png](/images/4.png)

2. Select your .pem file **(ex. amazonec2_keypair_virginia.pem)**, and then click **Open**. Click **OK** to dismiss the confirmation dialog box.

3. Click **Save private key** to save the key in the format that PuTTY can use. PuTTYgen displays a warning about saving the key without a passphrase, click **Yes**.

4. Specify the same name for the key that you used for the key pair **(ex. amazonec2_keypair_virginia.ppk)**. PuTTY automatically adds the .ppk extension.

5. Start **PuTTY.exe**, enter **Host Name**, find hostname from AWS console. (select Lab Server, and copy the **public IP** value.).

![5.png](/images/5.png)

![6.png](/images/6.png)

6. On the navigation pane, click **Connect>SSH>Auth**, click **Browse** to choose your key pair (ex.**amazonec2_keypair_virginia.ppk**), click **Open**.

![7.jpg](/images/7.jpg)

7. Enter **ec2-user**,and press ENTER.You are now logged into your **Lab Server** instance.

![8.png](/images/8.png)
