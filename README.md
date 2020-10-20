# This is a guide to set up ssh connection between git and github
## Generate ssh key on localhost first
### create a github account

- copy the ssh key from localhost with

`
cat id_rsa.pub
`

- paste the public key on your github in settings GPG SSH key option in your
  profile
- once saved go back to your terminal
- run the git hub command
`

git add .
git commit -m "name"
git push -u origin main
`

 - Download Git or GitBash (Mac and Linux has it already)
 - Make a folder using mkdir
 - Example: mkdir Engineering74
 - Go to the folder just created using 'cd Engineering74'
 - Generate a key: ssh-keygen -t rsa -b 4096 -C "your_email@email.com"
 - Save as "key.ssh"
 - Make a passphase (Optional but good practice)
 - Check that key.ssh exists with ls in you Engineering74 folder
 - Ensure you have git-agent eval $(ssh-agent -s)
 - Add the key ssh-add key.ssh
 - Go to your Github and go to Settings: "SSH and GPG keys" => "New SSH Key"
 - Go back to terminal and find the key with cat key.ssh.pub
 - Copy the key you see in terminal
 - Paste it in your New SSH Key window
