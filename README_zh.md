# Soundness 测试网
[English](https://github.com/walirt/soundness-testnet/blob/main/README.md) | 中文

## 8皇后游戏
1. 在 [Soundess Discord](https://discord.gg/soundnesslabs) 的 🕹️#game-arena 频道发送 `/8queens` 命令
![](https://github.com/walirt/soundness-testnet/blob/main/1.png?raw=true)
2. 在回复的消息内点击 Launch Game 打开网站
![](https://github.com/walirt/soundness-testnet/blob/main/2.png?raw=true)
3. 参考以下图片放置棋子完成游戏，完成后会收到 Sound_Game 机器人的私聊信息
![](https://github.com/walirt/soundness-testnet/blob/main/3.png?raw=true)
4. 点击 `Generate Ligero Proof` 按钮生成证明，完成后将自动获得 Discord `Sound OG` 角色
![](https://github.com/walirt/soundness-testnet/blob/main/4.png?raw=true)
5. 点击证明消息复制命令按钮复制命令
![](https://github.com/walirt/soundness-testnet/blob/main/5.png?raw=true)
6. 打开服务器，确保你已经安装docker，运行以下命令
    ```bash
    # 拉取 soundness-cli 镜像
    docker pull walirt/soundness-cli:v0.1.2
    cd && mkdir soundness
    # 添加别名
    alias soundness-cli="docker run -it --rm -v $PWD:/app walirt/soundness-cli:v0.1.2" 
    ```

7. 如果你有保存之前在 Discord 绑定的钱包助记词，运行以下命令导入
    ```bash
    # 导入助记词
    soundness-cli import-key --name 钱包名字 --mnemonic "助记词"
    # 查看所有钱包
    soundness-cli list-keys
    ```
8. 如果你丢失了之前在 Discord 绑定的钱包助记词，运行以下命令重新生成
    ```bash
    # 生成新钱包
    soundness-cli generate-key --name 钱包名字
    # 查看所有钱包
    soundness-cli list-keys
    ```
9. 粘贴之前在复制的命令，把 `<your-key-name>` 修改成上面的钱包名字
![](https://github.com/walirt/soundness-testnet/blob/main/6.png?raw=true)
10. 回显消息为 `Status: SUCCESS` 则为成功，可以打开 `Suiscan Link` 链接查看TX
![](https://github.com/walirt/soundness-testnet/blob/main/7.png?raw=true)

## 联系我
[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/walirttt.svg?style=social&label=关注%20%40walirttt)](https://twitter.com/walirttt)