# truffle-docker-environment
truffle docker environment

這是拿來練習 ethereum smart contract 的 docker 環境，自己也還在實驗中就是了 :p

## 安裝
1. 先複製 `.env.example` 為 `.env`，並在 `.env` 裡面加入你的基本設定
    ```
    $ cp .env.example .env
    ```
    之後再 `.env` 裡面設定 image name 跟你的 smart contract 擺放的位置

2. 開始 build 你的 image
    ```
    $ docker-compose build
    ```

3. 啟動每個 container
    ```
    $ docker-compose up -d
    ```

4. 啟動完之後，就可以進入 truffle 裡去 unbox `webpack` OR `react`
    ```
    $ docker-compose exec truffle bash
    ```

5. 進入 truffle 之後，default work dir 在 `/Ethereum` 下
    ```
    $ root@012aa9fd4a1a:/Ethereum#
    $ root@012aa9fd4a1a:/Ethereum# truffle unbox webpack
    ```

so, 環境好了之後，接下來再看看要怎麼玩好了
