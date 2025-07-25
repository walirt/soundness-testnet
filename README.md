# Soundness testnet
English | [中文](https://github.com/walirt/soundness-testnet/blob/main/README_zh.md)

## 8 Queens Game
1. Send `/8queens` command in the 🕹️#game-arena channel of [Soundess Discord](https://discord.gg/soundnesslabs)  
![](https://github.com/walirt/soundness-testnet/blob/main/1.png?raw=true)
2. Click "Launch Game" in the reply message to open the website  
![](https://github.com/walirt/soundness-testnet/blob/main/2.png?raw=true)
3. Refer to the following images to place the pieces and complete the game. After completion, you will receive a DM from the Sound_Game bot  
![](https://github.com/walirt/soundness-testnet/blob/main/3.png?raw=true)
4. Click the `Generate Ligero Proof` button to generate proof. After completion, you will automatically receive the Discord `Sound OG` role  
![](https://github.com/walirt/soundness-testnet/blob/main/4.png?raw=true)
5. Click the copy command button in the proof message to copy the command  
![](https://github.com/walirt/soundness-testnet/blob/main/5.png?raw=true)
6. Open your server, make sure you have Docker installed, and run the following commands  
    ```bash
    # Pull soundness-cli image
    docker pull walirt/soundness-cli:v0.1.2
    cd && mkdir soundness
    # Add alias
    alias soundness-cli="docker run -it --rm -v $PWD:/app walirt/soundness-cli:v0.1.2" 
    ```

7. (Option 1) If you have saved the wallet mnemonic phrase previously bound in Discord, run the following command to import it  
    ```bash
    # Import mnemonic phrase
    soundness-cli import-key --name wallet-name --mnemonic "mnemonic phrase"
    # View all wallets
    soundness-cli list-keys
    ```

8. (Option 2) If you lost the wallet mnemonic phrase previously bound in Discord, run the following command to regenerate it  
    ```bash
    # Generate new wallet
    soundness-cli generate-key --name wallet-name
    # View all wallets
    soundness-cli list-keys
    ```

9. Paste the previously copied command, and replace `<your-key-name>` with the wallet name from above  
![](https://github.com/walirt/soundness-testnet/blob/main/6.png?raw=true)
10. If the response message shows `Status: SUCCESS`, it means success. You can open the `Suiscan Link` to view the TX  
![](https://github.com/walirt/soundness-testnet/blob/main/7.png?raw=true)

## Contact Me
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/walirttt.svg?style=social&label=Follow%20%40walirttt)](https://twitter.com/walirttt) 