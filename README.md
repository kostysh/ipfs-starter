# ipfs-starter
The ease way to start local IPFS server with Docker

## IPFS start
```sh
npm start
```
- IPFS host will be started and listen to connections on ports `4001`  and `5001`.  
- Web browser will be accessible via `http://localhost:9090/ipfs/<object_hash>`
- Local IPFS database will be mapped to the folder `/.ipfs` 
- Transit folder for files `/.ipfs-export`

## Exec IPFS commands
```sh
npm run exec -- <args...>
```
For example: connect to peers  
```sh
npm run exec -- connect to peers
```
## Add files
```sh
cp -r <something> /.ipfs-export
npm run exec -- add -r /export/<something>
```

## IPFS stop
```sh
npm run stop
```
