# 2️⃣ 2. Git Setup and GitHub Desktop

# Set up Git

At the heart of GitHub is an open source version control system (VCS) called Git. Git is responsible for everything GitHub-related that happens locally on your computer.

To use Git on the command line, you'll need to download, install, and configure Git on your computer.


1. **Download and install the latest version of Git** 


    apt-get install git

or visit  `https://git-scm.com/downloads`


2. **Set your username/email in Git.**


    $ git config --global user.name "Mona Lisa"
    $ git config --global user.email "email@example.com"

Confirm that you have set the email address correctly in Git:


    $ git config --global user.email
    >email@example.com

**Done.** 

Git is now setup


## Authenticating with GitHub from Git

When you connect to a GitHub repository from Git, you'll need to authenticate with GitHub using either HTTPS or SSH.

**Connecting over SSH** 

If you clone GitHub repositories using SSH, then you authenticate using SSH keys instead of a username and password. 

Add a public key to your user account in the account settings page 

`https://github.com/settings/keys`

***After adding your public key to your GitHub account you will never need to enter a username or password again.***

For help setting up an SSH connection, see [Generating an SSH Key](https://help.github.com/en/articles/generating-an-ssh-key).

Checking for existing SSH keys


    $ ls -al ~/.ssh
    # Lists the files in your .ssh directory, if they exist

Generating a new SSH key and adding it to the ssh-agent


    $ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

Enter the **filename** (use github in the name to indicate this key is used for github) press Enter. 


    > Enter a file in which to save the key (~/.ssh/id_github): [Press enter]

At the prompt, type a **passphrase**. 


    > Enter passphrase (empty for no passphrase): [Type a passphrase]
    > Enter same passphrase again: [Type passphrase again]

Adding your SSH key to the ssh-agent

If your ssh-agent is not currently running, then start it again


    $ eval "$(ssh-agent -s)"
    > Agent pid 59566

Add your SSH private key to the ssh-agent


    $ ssh-add ~/.ssh/id_rsa


**Test your connection to GitHub**

After you've set up your SSH key and added it to your GitHub account, you can test your connection.


    $ ssh -T git@github.com
    # Attempts to ssh to GitHub

If everything is correct


    > Hi username! You've successfully authenticated, but GitHub does not
    > provide shell access.

If there was an error the most often mistake people make is forgetting to add the new key to the ssh-agent.  


**Connecting over HTTPS** 

If you [clone with HTTPS](https://help.github.com/en/articles/which-remote-url-should-i-use/#cloning-with-https-urls-recommended), you can [cache your GitHub password in Git](https://help.github.com/en/articles/caching-your-github-password-in-git) using a credential helper.
[Connecting over SSH](https://help.github.com/en/github/getting-started-with-github/set-up-git#connecting-over-ssh)

Turn on the credential helper so that Git will save your password in memory for some time. By default, Git will cache your password for 15 minutes.

1. In Terminal, enter the following:

    $ git config --global credential.helper cache
    # Set git to use the credential memory cache

2. To change the default password cache timeout, enter the following:

    $ git config --global credential.helper 'cache --timeout=3600'
    # Set the cache to timeout after 1 hour (setting is in seconds)





## Using Git Desktop

if you want to work with Git locally, but don't want to use the command line, you can instead download and install the [GitHub Desktop](https://desktop.github.com/) client.  For Download for macOS Windows (msi)



![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1585854819646_github-desktop-screenshot-windows.png)


`https://github.com/desktop/desktop`
`https://desktop.github.com/`

 For more information, see "[Getting started with GitHub Desktop](https://help.github.com/en/desktop/guides/getting-started-with-github-desktop)."

If you don't need to work with files locally, GitHub lets you complete many Git-related actions directly in the browser, including:


- [Creating a repository](https://help.github.com/en/articles/create-a-repo)
- [Forking a repository](https://help.github.com/en/articles/fork-a-repo)
- [Managing files](https://help.github.com/en/articles/managing-files-on-github)
- [Being social](https://help.github.com/en/articles/be-social)



![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320388_Screenshot+from+2020-04-10+13-48-22.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320404_Screenshot+from+2020-04-10+13-48-58.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320416_Screenshot+from+2020-04-10+13-49-49.png)

![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320425_Screenshot+from+2020-04-10+13-50-08.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320435_Screenshot+from+2020-04-10+13-50-32.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320447_Screenshot+from+2020-04-10+13-51-32.png)

![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320455_Screenshot+from+2020-04-10+13-51-48.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320465_Screenshot+from+2020-04-10+13-53-27.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320476_Screenshot+from+2020-04-10+13-53-45.png)

![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320486_Screenshot+from+2020-04-10+13-54-31.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320515_Screenshot+from+2020-04-10+13-54-41.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320499_Screenshot+from+2020-04-10+13-55-15.png)

![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320527_Screenshot+from+2020-04-10+13-55-50.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320538_Screenshot+from+2020-04-10+13-57-13.png)
![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320554_Screenshot+from+2020-04-10+13-57-37.png)

![](https://paper-attachments.dropbox.com/s_FCB1254488908366E9184B764B17408E9D2E7ECD6E1730B08D9447B453F4295B_1586561320571_Screenshot+from+2020-04-10+13-59-14.png)


