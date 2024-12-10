## General Benchmarks

### Geekbench 6

| Geekbench CPU                                          | Single-core | Milti-core |
| ------------------------------------------------------ | ----------- | ---------- |
| [MacOS](https://browser.geekbench.com/v6/cpu/9332803)  | 1521        | 6820       |
| Windows                                                |             |            |
| [Ubuntu](https://browser.geekbench.com/v6/cpu/9340751) | 1629        | 7252       |

### Sysbench
[source](https://wiki.gentoo.org/wiki/Sysbench)

```bash
sysbench --test=fileio --file-total-size=128G prepare
sysbench --test=fileio --file-total-size=128G --file-test-mode=rndrw --max-time=300 --max-requests=0 run
sysbench --test=fileio --file-total-size=128G cleanup 
```

| fileio      | read MiB/s | written MiB/s | 
| ----------- | ---------- | ------ |
| MacOS       | 40.04   | 26.69   |
| Windows     |         |         |
| Ubuntu      |     |  |    

```bash
sysbench --test=memory --num-threads=4 run
```

| memory  | operations/second | transfer speed MiB/s | 
| ------- | ----------------- | -------------------- | 
| MacOS   | 10080107.3        | 9853.85              |
| Windows |               |         |
| Ubuntu  | 10911563.3        | 10655.83             |

### Novabench
| Cinebench 2024 | CPU Score | GPU Score | Memory Score | Storage Score |
| -------------- | --------- | --------- | ------------ | ------------- | 
| MacOS          | 780       | 225       | 267          | 280           | 
| Windows        |           |           |              |               | 
| Windows        | 1180      | 200       | 423          | 256           | 

### Cinebench
| Cinebench 2024 | Single Core | Multicore | Ratio |
| -------------- | ----------- | --------- | ----- |
| MacOS          | 72          | 570       | 7.89x | 
| Windows        |             |           |       |   

## Graphic Benchmarks

| Geekbench GPU | Metal      | Vulkan     | OpenCL     | 
| ------------- | ---------- | ---------- | --------------------------------------------------------- |
| MacOS         | [37933](https://browser.geekbench.com/v6/compute/3289995) |            | [24114](https://browser.geekbench.com/v6/compute/3289934) |
| Windows       |            |            |            |
| Ubuntu        |            | [46962](https://browser.geekbench.com/v6/compute/3292510) |            |

Valley Benchmark (1080p high opengl) 

| memory  | Score | FPS | 
| ------- | ---- | ----- | 
| MacOS   | 3542 | 84.7  |
| Windows |      |       |
| Ubuntu  | 3137 | 75.0  |


## Browser Benchmarks 

### Basemark Web 3.0

| Basemark Web 3.0 | Firefox | Edge    | Safari   |
| ---------------- | ------- | ------- | -------- |
| MacOS            | 859.59  | 705.9   | 762.87   |
| Windows          |         |         |          |
| Ubuntu           | 1346.65 | 1329.66 |          |

### WebXPRT 4

| WebXPRT 4        | Firefox | Edge    | Safari   |
| ---------------- | ------- | ------- | -------- |
| MacOS            | 199     | 210     | 197      |
| Windows          |         |         |          |
| Ubuntu           | 215     | 198     |          |
