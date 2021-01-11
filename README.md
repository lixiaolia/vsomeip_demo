### VSOMEIP DEMO

可作为vsomeip的使用示例

#### Dependencies

编译和安装boost：

```bash
cd boost_1_57_0
./bootstrap.sh
./b2 link=shared
sudo ./b2 install
```

编译和安装vsomeip：

```bash
git clone https://github.com/GENIVI/vsomeip.git
cd vsomeip
mkdir build
cd build
cmake -DENABLE_SIGNAL_HANDLING=1 -DDIAGNOSIS_ADDRESS=0x10 ..
make
sudo make install
```


#### Compilation

```bash
mkdir build
cd build
cmake ..
make
```

