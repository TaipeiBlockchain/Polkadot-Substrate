## 當 Codenvy 環境成功建立後會自動開啟一個新 Terminal
```bash
cd ../projects/

cp -r /home/substrate-node-template/ .

source ~/.cargo/env

substrate-ui-new substrate

substrate-node-template/target/release/substrate-node-template --dev
```

## 開啟一個新 Terminal
```bash
/home/ngrok http 9944
```

## 修改 /projects/substrate-ui/src/index.js 中的 setNodeUri
```js
setNodeUri(['wss://xxxxx.ngrok.io/', 'wss://substrate-rpc.parity.io/'])
```
## 再開啟一個新 Terminal
```bash
cd projects/substrate-ui/

yarn install

yarn run dev
```
