# python_dunder_all_iall_speed_diff

## Run

```sh
$ task
task: [default] hyperfine "python dunder_add.py" "python dunder_iadd.py"
Benchmark 1: python dunder_add.py
  Time (mean ± σ):      1.210 s ±  0.018 s    [User: 0.835 s, System: 0.376 s]
  Range (min … max):    1.173 s …  1.233 s    10 runs
 
Benchmark 2: python dunder_iadd.py
  Time (mean ± σ):      79.2 ms ±   2.6 ms    [User: 46.4 ms, System: 34.7 ms]
  Range (min … max):    74.1 ms …  88.2 ms    37 runs
 
Summary
  python dunder_iadd.py ran
   15.27 ± 0.54 times faster than python dunder_add.py
```

## REFERENCES

- [a=a+b and a+=b are not always same in Python](https://twitter.com/Python_Dv/status/1709887657088598413?s=20)
- [Different behaviour for list.__iadd__ and list.__add__](https://stackoverflow.com/questions/9766387/different-behaviour-for-list-iadd-and-list-add)
