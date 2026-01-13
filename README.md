# GUIDE-TO-CREATE-FIRST-GENLAYER-CONTRACT

Deploying a smart contract with the genlayer studio takes years
This will help you setup a GenLayer cli and host the studio without needing a validator

# Requirements
1. docker
2. python v3.10+
3. node.js v18+
4. ubuntu

## STEP ONE
### installing ubuntu
  - open up windows powershell as an administrator
    <img width="1366" height="601" alt="image" src="https://github.com/user-attachments/assets/b8a4a46f-f7cc-4957-8b5e-d1fc30e3e169" />
  - type in

<pre>
  wsl
</pre>

after it installs, you have to reboot
it then asks for your password

## STEP TWO
### install python
- update your pkg list: 
<PRE>
  sudo apt update
</PRE>

- check if you have it installed already:
<PRE>
  python3 --version
</PRE>

- if not then install it; 
<PRE>
  sudo apt install python3
</PRE>

- add pip too;
<PRE>
  sudo apt install python3-pip
</PRE>

## STEP THREE
### install cURL
<PRE>
  sudo apt update
sudo apt install curl
</PRE>

- add nVM
<PRE>
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
</PRE>

- close your terminal and open again as admin;
  RUN
  <PRE>
    nvm install 18
  </PRE>

- verify your node version with
<PRE>
  node -v
</PRE>

## INSTALL DOCKER ON YOUR PC
visit: docs.docker.com/desktop/setup/install/windows-install 
download that which suites your pc
<img width="1265" height="564" alt="image" src="https://github.com/user-attachments/assets/a86159fc-66dd-424a-ab5c-34c6a0bd7cf8" />


### after all the requirements are setup;
- open docker
- open powershell and run;
<pre>
  wsl
</pre>
<img width="1362" height="551" alt="image" src="https://github.com/user-attachments/assets/fd64f39d-0fd4-4acc-883d-57955d6eef15" />

# Let's setup the genlayer client, so we can deploy contracts on our own (remember always open ubuntu in powershell with wsl command)

## install genlayer cli to work as blockchain simulator
<pre>
  npm install -g genlayer
</pre>
<img width="680" height="383" alt="image" src="https://github.com/user-attachments/assets/e326b563-fdee-4642-b56d-40a569ed205c" />

## initialize node/blockchain environment
first you will create a folder for your work to run on.
example; i want a create a vibe checker project, so i name my folder using (mkdir foldername)
<pre>
  mkdir vibe-check-oracle
</pre>

- now, go to this folder;
  <pre>
    cd vibe-check-oracle
  </pre>

  - initialize the cli now;
  <pre>
    genlayer init
  </pre>

note: it will prompt you that some files will be deleted except some
answer with "Y"
then, you will be asked to select an LLM and also provide api keys
<img width="680" height="328" alt="image" src="https://github.com/user-attachments/assets/a0f9c803-8aa0-4cf4-9187-053e01ccfe6e" />

#### genlayer partnered with heurist ai to give free credits for this
visit: heurist. ai/credits (remove space hehe)
use the word "genlayer" as referral to get the free credits
<img width="680" height="297" alt="image" src="https://github.com/user-attachments/assets/65a9ec39-2905-46da-b4c5-930f283bbd7b" />

- back to your terminal; navigate to heaurist ai, use your space bar to select it and ENTER to approve
- get your api key from heurist ai and right click to paste and then enter

## start node
- after initialization succeeds, run this command
<pre>
  genlayer up
</pre>

if this runs successfully, you see a localhost url with 8080
<img width="680" height="166" alt="image" src="https://github.com/user-attachments/assets/89864ff4-0be1-4160-87d8-2cb3f2d9f59e" />

## visit your personal studio and deploy contract
open your browser and visit: http://localhost:8080
you should be welcomed by the genlayer studio

<img width="680" height="274" alt="image" src="https://github.com/user-attachments/assets/e62d90e3-72cf-4fe4-9751-a597d594595f" />

create a contract file
paste your contract code in the terminal and deploy
this works easily

#### now you can copy your contract address and continue building on genlayer

