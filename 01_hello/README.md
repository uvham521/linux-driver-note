# 01_hello

简单的 HelloWorld 驱动模块

执行 `make` 编译代码。

## 使用方法

开启两个终端，这样可以边操作边查看内核日志，观察结果。

- 在终端 A 中，持续打印新的内核日志
  ```
  sudo dmesg -w
  ```
- 在终端 B 中，加载模块

  ```
  sudo insmod hello.ko
  ```

- 此时，终端 A 中会显示 Hello 日志

  ```
  [ 6120.500778] hello - Hello, Kernel!
  ```

- 在终端 B 中，卸载模块

  ```
  sudo rmmod hello
  ```

- 此时，终端 A 中会显示 Goodbye 日志

  ```
  [ 6201.413744] hello - Goodbye, Kernel!
  ```

## 补充命令

- 查看模块信息

  ```
  modinfo ./hello.ko
  ```

- 列出已经加载的模块

  ```
  lsmod
  ```

- 另一个模块加载命令（加载模块的同时加载所依赖的其他模块）

  ```
  modprobe hello.ko
  ```
