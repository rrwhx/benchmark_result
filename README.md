## kernel build
```bash
# download from https://mirrors.edge.kernel.org/pub/linux/kernel/
time tar -xf linux-5.15.46.tar.xz
make defconfig
time make -jN
```

|  platform |unzip time   |  build time  |  kernel version | gcc version  | comment  |
| :------------: | :------------: | :------------: | :------------: | :------------: | :------------: |
|  12700k | 5.35  | 59.29  | 5.15.46  | 11.2.0  | -j20  |
|  EPYC 7543 * 2 | 6.52  |  24.98    | 5.15.46  | 9.4.0  | -j128  |
|   |   |   |   |   |   |

## octane
[https://chromium.github.io/octane/](https://chromium.github.io/octane/ "https://chromium.github.io/octane/")
[http://180.76.245.10/octane/](http://180.76.245.10/octane/ "http://180.76.245.10/octane/")

| platform  | score   | browser  | os  | comment  |
| :------------: | :------------: | :------------: | :------------: | :------------: |
| 12700k  | 84298  | chrome 102.0.5005.115  | ubuntu22.04 with kernel 5.15.0-33-generic  |   |
| Loongson 3A 4000  | 8224  |  3.1.5259.1 | 90.0.4430.217 | loongnix with kernel 4.19.190  |   |
|   |   |   |   |   |


