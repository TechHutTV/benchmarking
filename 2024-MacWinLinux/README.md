## General Benchmarks

MacBook Pro Retina 16-inch (2019) - Core i9 - 16GB - SSD 1000GB

Processor
Intel Core i9-9880H 2.3Ghz

Graphic Card Type
AMD Radeon Pro 5500M

Resolution
3072 x 1920

### Geekbench 6

Geekbench is a common tool for testing the performance of devices like phones, laptops, and tablets. It can provide insights into how a device will perform with professional applications that require high levels of processing power. It measures both single-core and multi-core power, and aggregates data from thousands of users to create an average score.

| Geekbench CPU                                           | Single-core | Milti-core |
| ------------------------------------------------------- | ----------- | ---------- |
| [MacOS](https://browser.geekbench.com/v6/cpu/9332803)   | 1521        | 6820       |
| [Windows](https://browser.geekbench.com/v6/cpu/9390869) | 1530        | 6284       |
| [Ubuntu](https://browser.geekbench.com/v6/cpu/9340751)  | 1629        | 7252       |

### Novabench

Novabench's tests are designed to evaluate modern API, instruction set, and workload performance. The results are comparable across operating systems and architectures.

| Cinebench 2024 | CPU Score | GPU Score | Memory Score | Storage Score |
| -------------- | --------- | --------- | ------------ | ------------- | 
| MacOS          | 780       | 225       | 267          | 280           | 
| Windows        | 1470      | 210       | 274          | 270           | 
| Ubuntu         | 1180      | 200       | 423          | 256           | 

### Sysbench

When using the memory test in sysbench, the benchmark application will allocate a memory buffer and then read or write from it, each time for the size of a pointer. [source](https://wiki.gentoo.org/wiki/Sysbench)

```bash
sysbench --test=memory --num-threads=4 run
```

| memory  | operations/second | transfer speed MiB/s | 
| ------- | ----------------- | -------------------- | 
| MacOS   | 10080107.3        | 9853.85              |
| Ubuntu  | 10911563.3        | 10655.83             |

### Cinebench
| Cinebench 2024 | Single Core | Multicore | Ratio |
| -------------- | ----------- | --------- | ----- |
| MacOS          | 1150        | 9041      | 7.86  |
| Windows        | 1145        | 7870      | 6.87  |

## Graphic Benchmarks

| Geekbench GPU | Metal      | Vulkan     | OpenCL     | 
| ------------- | ---------- | ---------- | --------------------------------------------------------- |
| MacOS         | [37933](https://browser.geekbench.com/v6/compute/3289995)              |            | [24114](https://browser.geekbench.com/v6/compute/3289934) |
| Windows       |            | [36842](https://browser.geekbench.com/v6/compute/3308764)              | [32920](https://browser.geekbench.com/v6/compute/3308755) |
| Ubuntu        |            | [46962](https://browser.geekbench.com/v6/compute/3292510) |            |

Valley Benchmark (1080p high opengl) 

| Valley               | Score | FPS   | 
| -------------------- | ----- | ----- | 
| MacOS (OpenGL)       | 3542  | 84.7  |
| Windows (OpenGL)     | 3162  | 75.6  |
| Windows (DirectX 11) | 3881  | 92.8  |
| Ubuntu (OpenGL)      | 3137  | 75.0  |


## Browser Benchmarks 

### Basemark Web 3.0

| Basemark Web 3.0 | Firefox | Edge    | Safari   |
| ---------------- | ------- | ------- | -------- |
| MacOS            | 859.59  | 705.9   | 762.87   |
| Windows          | 1093.43 | 1096.69 |          |
| Ubuntu           | 1346.65 | 1329.66 |          |

### WebXPRT 4

| WebXPRT 4        | Firefox | Edge    | Safari   |
| ---------------- | ------- | ------- | -------- |
| MacOS            | 199     | 210     | 197      |
| Windows          | 190     | 185     |          |
| Ubuntu           | 215     | 198     |          |
