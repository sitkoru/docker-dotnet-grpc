# docker-dotnet-grpc

Docker image with latest .NET Core SDK, protobuf compiler and grpc plugin to build and compile .NET classes from .proto files.

# GRPC version

v1.19.0

# Usage

```
find protobuf_dir -name "*.proto" | xargs /usr/local/bin/protoc --csharp_out=CS_DIR --proto_path=include --proto_path=protobuf_dir
dotnet pack
```
