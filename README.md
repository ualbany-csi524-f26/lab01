# lab01
- Link to create your repository: (Link will be available in a few days. For now, please follow the instructions to prepare your setup.)
- Due Sep. 3, 2026
- Final contents of your repository:
  - `screenshot.png`

---
In this lab you set up your personal virtual machine and customize its terminal prompt (required for all following labs).

## Task 1: Set up VM
In this class, we will practice various security concepts and attacks based on an open-source project called SEED Labs. SEED Labs are based on a pre-built virtual machine in order to perform the labs more conveniently.

It is highly recommended that you use a virtual machine rather than your own operating system for these exercises. We often need to disable security countermeasures or configure lab machines in a way that makes them vulnerable. Furthermore, some of the labs have been designed specifically with the provided VM machine in mind. While concepts are universal, specific tasks/settings could be very different in a different environment.

Follow the [lab VM setup instructions](https://github.com/ualbany-csi524-f26/guides) in the guides. Note that if you have an Apple Silicon Mac, you need to follow a different set of instructions.

## Task 2: Set up GitHub access and clone your repository
Click on the link at the top of this lab to create your GitHub repository for this lab. 

Run your SEED Ubuntu machine and log in as user "seed". In order to use GitHub from shell, you need to either use an access token or SSH. Setting up a GitHub access token is simpler. If you are an advanced Linux user, you can alternatively set up an SSH access, which makes your life much easier. Follow the [links to the corresponding instructions](https://github.com/ualbany-csi524-f26/guides). 

Once your GitHub access is set up, clone your lab01-username repository to your SEED VM.

## Task 3: Customize your terminal prompt
In your SEED Ubuntu machine (as the seed user):

1. Open file `~/.bashrc` using your favorite text editor (`gedit`, `nano`, etc.)
2. Locate all lines that start with word `PS1=`. For example:
    ```
    PS1='[`date "+%D"`]\u@\h:\w\$ '
    ```
3. Modify such lines by inserting a hyphen and your 8-charachter NETID (e.g., "-XY123456") after `\u` in the lines. The above example will be modified to:
    ```
    PS1='[`date "+%D"`]\u-XY123456@\h:\w\$ '
    ```
4. Save and close the file.
5. Reload your `.bashrc` by running the following. Make sure that you see the updated prompt in your terminal.
    ```
    source ~/.bashrc
    ```
6. Finally, run the following command, take a screenshot of the terminal, and save it as `screenshot.png`:
    ```
    uname -a
    ```   
7. Include `screenshot.png` in your repository.

## Task 4: "Submit" your assignment
Make sure that you commit and push from your local repository to our GitHub organization once you are done with your lab. Your final commit in your repository on GitHub serves as your submission.
