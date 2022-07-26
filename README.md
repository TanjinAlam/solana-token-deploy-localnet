#### Local-Server

- Run Following Command
```
solana-keygen new 
solana config set --url localhost
solana-test-validator
```


#### Deploy Token

- Run Following Command
```
cargo build-bpf --manifest-path=./Cargo.toml --bpf-out-dir=dist/program
solana program deploy dist/program/token_program.so
npm run start
```