# S2
```
curl -O https://github.com/protocolbuffers/protobuf/releases/download/v3.19.4/protoc-3.19.4-osx-x86_64.zip
unzip protoc-3.19.4-osx-x86_64.zip -d /usr/local/protobuf
# or
sudo mv protoc-3 /usr/local/protobuf

go get google.golang.org/protobuf/...@v1.25.0

protoc api/v1/*.proto \
    --go_out=. \
    --go_opt=paths=source_relative \
    --proto_path=.

# for M1
https://repo1.maven.org/maven2/com/google/protobuf/protoc/3.19.2/
```