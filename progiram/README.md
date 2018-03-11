```
cc -o hello hello.c
strace -o hello.log ./hello
```

- taskset
  - コマンドライン引数で指定したプログラムを-cオプションによって指定した論理CPU上でのみ動作させる
  - `taskset -c 0 ./sched <n> <total> <resol>`
