# corechain
从零开始用nodejs写一个区块链

安装相关库 npm intall 

启动代码 npm run start

打开另一个窗口 分别执行以下命令 ，观察第一个窗口的输出


获取一个 blockchain

curl http://localhost:3001/blocks


创建 block

curl -H "Content-type:application/json" --data '{"data" : "Some data to the first block"}' http://localhost:3001/mineBlock



添加 peer

curl -H "Content-type:application/json" --data '{"peer" : "ws://localhost:6001"}' http://localhost:3001/addPeer


连接peers

curl http://localhost:3001/peers
