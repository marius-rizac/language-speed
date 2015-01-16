
## Run PHP (5.5.9) 
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do php a.php >/dev/null ; i=$(($i-1)); done )
```

### Result
<pre>
real    1m52.333s
user    1m14.740s
sys     0m36.947s
</pre>

## Run Python (2.7.6)
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do python b.py >/dev/null ; i=$(($i-1)); done )
```

### Result
<pre>
real    0m40.247s
user    0m27.252s
sys     0m13.178s
</pre>

## Run Python (3.4.0)
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do python3 b3.py >/dev/null ; i=$(($i-1)); done )
```

### Result
<pre>
real    1m6.288s
user    0m53.569s
sys     0m12.576s
</pre>

## Run Ruby
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do ruby c.rb >/dev/null ; i=$(($i-1)); done )
```

### Result
<pre>
real    0m41.135s
user    0m27.719s
sys     0m9.803s
</pre>

