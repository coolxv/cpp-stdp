# Centos上升级GCC(Tested on Centos 8.3)

https://access.redhat.com/documentation/zh-cn/red_hat_enterprise_linux/8/html-single/developing_c_and_cpp_applications_in_rhel_8/index

```
1.安装 GCC Toolset 版本 N:
  # yum install gcc-toolset-N

2.从 GCC Toolset 安装单独的软件包
  列出 GCC Toolset 版本 N 中的可用软件包：
  $ yum list available gcc-toolset-N-\*

  安装这些软件包：
  # yum install package_name
  使用空格分开的软件包列表替换 package _name。例如,要安装 gcc-toolset-9-gdb-gdbserver 和 gcc-toolset-9-gdb-doc 软件包：

  # yum install gcc-toolset-9-gdb-gdbserver gcc-toolset-9-gdb-doc

3.卸载 GCC Toolset 版本 N:
  # yum remove gcc-toolset-N\*

4.要从 GCC Toolset 版本 N 运行工具：
  $ scl enable gcc-toolset-N tool

5.要运行来自 GCC Toolset 版本 N 的工具版本的 shell 会话,覆盖这些工具的系统版本：
  $ scl enable gcc-toolset-N bash
```