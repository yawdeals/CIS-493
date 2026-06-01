# CIS-493


 type -p curl >/dev/null || sudo apt install curl -y
 curl -fsSL https://cli.github.com/packages/githubcli-archive-keyring.gpg | \
   sudo dd of=/usr/share/keyrings/githubcli-archive-keyring.gpg
 sudo chmod go+r /usr/share/keyrings/githubcli-archive-keyring.gpg
 echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/githubcli-archive-keyring.gpg] https://cli.github.com/packages stable main" | \
   sudo tee /etc/apt/sources.list.d/github-cli.list > /dev/null
 sudo apt update
 sudo apt install gh

2. Authenticate with GitHub:

 gh auth login

3. Install the Copilot extension:

 gh extension install github/gh-copilot

4. Authenticate Copilot:

 gh copilot auth login

Now you can use Copilot in your terminal with commands like:

 gh copilot suggest "Write a bash script that prints Hello World"



 type -p curl >/dev/null || sudo apt install curl -y
