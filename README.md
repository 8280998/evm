# evmEVM通用交互程序
说明：适用于大部分EVM网络批量刷tx。可以自行在cnofig.json添加不同链的rpc和链id。

2025-10-25 更新：在gui界面增加了发送eth的参数，默认为0.因为有些mint nft需要发送少量eth到交互合约才能mint成功。

## 已在以下网络部署的交互合约
### 1 monad测试网 链选择:monadtestnet
空投领取测试币，交互合约地址：0xfcBA9b0ABc504bCBb89F0771833c57F17FDbdd42

data：0x4e71d92d

测试币应用游戏web：https://monad-bet-game.vercel.app/

### 2 giwa测试网 链选择：giwatestnet
空投领取测试币，交互合约地址：0xf931b1dAFdebC98b5cBdF5EC5fE043e81CDf8559

data：0x4e71d92d

测试币应用游戏web：https://giwagame.vercel.app/

<img width="1188" height="642" alt="image" src="https://github.com/user-attachments/assets/9ee82e27-121c-42da-b6ec-c9be9259f4c7" />



## 免责声明：本程序为明文代码，运行前请先审核代码安全性。确定使用后，运行时产生任何损失均与本代码无关

## 1 安装支持环境
安装 Python，tkinter（GUI 库）， web3（区块链交互库）

    sudo apt update && sudo apt install python3 python3-pip
    sudo apt install python3-tk
    pip3 install web3

## 2 准备私匙文件和配置文件
程序读取私匙文件address.txt内容，一行一个。类似如下：

0x123456...

config.json如果不包括需要的网络，请自行在config.json中添加所需网络。


## 3 运行脚本
    python3 evm.py

在弹出的窗口中设置参数，选择链和交互目标的合约地址。发送的data。如下图是刷monad运行
    
## 4 运行截图如下
<img width="1200" height="1056" alt="image" src="https://github.com/user-attachments/assets/b3c14b95-52c1-47e0-ad84-ee0bc1b78ad6" />


增加发送eth参数后，运行。下图是在giwa测试网 mint一个nft。每个nft需要支付0.001eth
<img width="1400" height="1056" alt="QQ_1760836454145" src="https://github.com/user-attachments/assets/f62362cf-d1bf-41c2-af6a-f073d2ff5ae1" />
