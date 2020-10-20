# This is a guide to set up ssh connection between git and github

 - Download Git or GitBash (Mac and Linux has it already)
 - Make a folder using mkdir
 - Example: mkdir Engineering74
 - Go to the folder just created using 'cd Engineering74'
 - Generate a key: ssh-keygen -t rsa -b 4096 -C "your_email@email.com"
<<<<<<< HEAD
 - Save as "key.ssh"
 - Make a passphase (Optional butgood practice)
 - Check that key.ssh exists with ls in you Engineering74 folder
 - Ensure you have git-agent eval $(ssh-agent -s)
 - Add the key ssh-add key.ssh
 - Go to your Github and go to Settings: "SSH and GPG keys" => "New SSH Key"
 - Go back to terminal and find the key with cat key.ssh.pub
 - Copy the key you see in terminal
 - Paste it in your New SSH Key window
=======
  Save as "key.ssh"
  Make a passphase (Good practice)
  SHA256:YOUR_KEY_HERE your_email@email.com
  Check that key.ssh exists with ls in your Sparta folder
  Ensure you have git-agent eval $(ssh-agent -s)
  Add the key ssh-add key.ssh
  Go to your Github and go to Settings
  "SSH and GPG keys" => "New SSH Key"
  Back to terminal cat key.ssh.pub
  Copy the entire thing you see in terminal
  Paste it in your New SSH Key window and add a title
  Back to terminal test your SHH to GitHub
  ssh -T git@github.com
  When you get RSA Key fingerprint question => yes
  If you see "Hi USER! You've Successfully authenticated..." = GOOD
  Save it => Profit £££
  Hide your key.ssh and key.ssh.pub somewhere safe
  NEVER LEAVE IT IN YOUR REPO FOLDER
  Step 1: Download 
>>>>>>> ecc1dd9120deb7e8d976adde4827a6c35b297824
