# Koii-Node-on-VPS
Thanks to @Pewd_Crypto &amp; @c-diamond for a tip

# Koii Task Node Setup on VPS

This tutorial guides you through the process of setting up a Koii task node on a Virtual Private Server (VPS). Follow the steps below to configure the environment and run the Koii task node.

_**## 1. Update and Install Dependencies**_

```bash
sudo apt update
sudo apt upgrade
sudo apt install git


**2. #Clone**
git clone https://github.com/koii-network/VPS-task
cd VPS-task



**3. #Download Koii CLI**
sh -c "$(curl -sSfL https://raw.githubusercontent.com/koii-network/k2-release/master/k2-install-init.sh)"


**4. #Check if Koii CLI is installed:**
koii --version


**5. #Config Testnet URL**
koii config set --url https://testnet.koii.live

6. #Check Balance
koii balance

**7. #Create New Wallet **
koii-keygen new -o /root/.config/koii/id.json


**7. #Import Wallet**
Watch This https://www.youtube.com/watch?v=h9LkcSo29IA at 9:22


**8. #Install Docker**
sudo apt install docker
docker-compose --version


**9. #Run Docker Compose**
Ensure you are in the VPS-Task directory:
docker-compose up

**10. #Run it on the background**
docker-compose up -d

11. #Check if it's running properly
docker logs -f --tail 10 task_node


**12. #Claim Reward**
sudo apt install npm
cd root
npx @_koii/create-task-cli@latest

For Example: Claiming Task ID 1: Free token Task!

Task ID: 6GbpHRK3duDbo3dCEFXuJ2KD5Hg6Yo4A9LyHozeE7rjN
StakePotAccount: FnQm11NXJxPSjza3fuhuQ6Cu4fKNqdaPkVSRyLSWf14d
Address that the funds will be transferred to: **your_wallet_address**
Path to claimer wallet: VPS-task/namespace/staking_wallet.json
