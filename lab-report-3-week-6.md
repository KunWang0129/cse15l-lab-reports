# This is Kun Wang CSE15L lab report 3

Kun Wang

Professor Soosai Raj

07 May 2022

_Streamlining ssh Configuration:_

- In this part of the lab, I have created my own config file that further simplified the login process for my ieng6 account.

![config](/lab3content/ssh_config.png)
- Now I can use `ieng6 Kun` to login to my ieng6 account.

![Kun_ssh](/lab3content/Kun_ssh.png)

- Here's another application of the simplified login command with copying a file to my account.

![scp_command](/lab3content/scp_command.png)

_Setup Girhub Access from ieng6_
- In this section, I have setup a key for Github Access from ieng6 account.
- Here is the public key shown in Github.

![github_key](/lab3content/publickey_github.png)

- Here is the public and private key stored in .ssh folder

![private/public_key](/lab3content/pub_privatekeys.png)

- Now we are going to use the key when we commit changes to Github from ieng6 account.

- Here is an example of a commit and push from ieng6 account to Github:

![ieng6_push/commit](/lab3content/remote_commit.png)

- Here is the link of the commit: [commitlink](https://github.com/KunWang0129/markdown-parser/commit/8d599ee2d089086f3025c9813ae0542b41547218)

_Copy whole directories_
- In this section we are going to copy an entire directory to ieng6 account
- Here a screenshot of the copying process
![scp_pt1](/lab3content/copydir_pt1.png)
![scp_pt2](/lab3content/copydir_pt2.png)

- Here is the directory copied in ieng6 account:

![scp_pt3](/lab3content/copydir_pt3.png)

- Next we are going to run the MarkdowmParseTest in the ieng6 account:

![ieng6_test](/lab3content/ieng6_test.png)

- Finally here we have the one line command that runs all steps in one line:

![oneline_pt1](/lab3content/oneLine_pt1.png)

![oneline_pt2](/lab3content/oneLine_pt2.png)





