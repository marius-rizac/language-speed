
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do php a.php >/dev/null ; i=$(($i-1)); done )
```

<pre>
real    1m52.333s
user    1m14.740s
sys     0m36.947s
</pre>

```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do python b.py >/dev/null ; i=$(($i-1)); done )
```

<pre>
real    0m40.247s
user    0m27.252s
sys     0m13.178s
</pre>

