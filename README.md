# UDP File Transfer

This is the homework of Chapter 6 of Computer Network Experiment 2024 in CUMT.

This repository Implemented file transfer via UDP protocol, with security check and beautified output.

## Development

The compile environment is MinGW, posix thread, C++ 20 standard on Windows OS. Please make sure you have Windows Kits on your computer.

If you meet problems when compiling, give a try to [LLVM MinGW](https://github.com/mstorsjo/llvm-mingw/releases).

To change the directory to save(default is `./received`), you can modify the `SAVE_PATH` in [udp_server.cpp](./udp_server.cpp).

The chunk for file transpotation is 1024 bytes, you can modify the `CHUNK_SIZE` in both [udp_server.cpp](./udp_server.cpp) and [udp_client.cpp](./udp_client.cpp).

> [!IMPORTANT]
> `CHUNK_SIZE` has to be modified in both files at the same time.

Moreover, `SOCKET_SND_TIMEOUT` and `SOCKET_RCV_TIMEOUT` is available to modify in [udp_server.cpp](./udp_server.cpp) and [udp_client.cpp](./udp_client.cpp), to set the timeout of the socket, in milliseconds.

## License

Copyright (c) Cnily03. All rights reserved.

Licensed under the [MIT](./LICENSE) License.
