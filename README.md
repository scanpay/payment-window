# Payment window

This repository contains the files used to generate the Scanpay Payment Window (paywin).

In 2022, we will open-source our payment window.

## Compatibility

We strive for maximum compatibility. 

| Feature               | DK %  | Edge | Firefox | Chrome | Safari | Opera | Safari iOS | Chrome for Android | Firefox for Android | Samsung Internet |
| --------------------- | ----- | ---- | ------- | ------ | ------ | ----- | ---------- | ------------------ | ------------------- | ---------------- |
| Const                 | 96.2% | 12   | 36      | 49     | 11     | 36    | 11         | 49                 | 36                  | 5                |
| TLS 1.2               | 96.1% | 12   | 27      | 29     | 7      | 16    | 5          | 29                 | 27                  | 4                |
| Let                   | 95.6% | 12   | 44      | 49     | 11     | 36    | 11         | 49                 | 44                  | 5                |
| KeyboardEvent.key     | 95.5% | 12   | 29      | 51     | 10.1   | 38    | 10.3       | 51                 | 29                  | 5                |
| Fetch                 | 94.9% | 14   | 39      | 42     | 10.1   | 29    | 10.3       | 42                 | 39                  | 4                |
| Arrow functions       | 94.8% | 12   | 22      | 45     | 10     | 32    | 10         | 45                 | 22                  | 5                |
| ~Async functions~ [1] | 94.1% | 15   | 52      | 55     | 11     | 42    | 11         | 55                 | 52                  | 6.2              |
| ~promise-finally~ [2] | 93.6% | 18   | 58      | 63     | 11.1   | 50    | 11.3       | 63                 | 58                  | 8.2              |
| ~TLS 1.3~ [3]         | 93.0% | 79   | 63      | 70     | 12.1   | 57    | 12.2       | 70                 | 63                  | 10.1             |

**[1]**: Async-await is not used yet, but we will use it in near the future.\
**[2]**: Finally is polyfilled.\
**[3]**: TLS 1.3 is supported, but older browsers can use TLS 1.2 (for now).\
