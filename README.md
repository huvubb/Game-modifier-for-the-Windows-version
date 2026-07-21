# GhostTrainer — 单机游戏内存修改器

v4.2 · 多线程并行扫描 · GPU 加速 · 内存安全系统

## 功能特性

- 12 路并行内存扫描（可自定义线程数 1-64）
- GPU 加速（OpenCL），CPU SIMD（SSE2）
- 支持 int8/int16/int32/int64/float/double
- 四种内存模式：激进 / 自适应 / 保守 / 自定义
- 16 套配色主题，6 档动画倍速
- 数值冻结功能
- 自动持久化配置
- 寻址宝典 & 地址图鉴
- 控制台 UTF-8 + VT 支持

## 编译

```bash
g++ -O3 -march=native -static -o GhostTrainer.exe GhostTrainer.cpp
```

## 数字签名

```powershell
signtool sign /fd SHA256 /f GhostTrainer.pfx /p gt123 /t http://timestamp.digicert.com GhostTrainer.exe
```
