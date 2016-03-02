## Run PHP (5.5.9) 
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do php a.php >/dev/null ; i=$(($i-1)); done )
```

## Run Python (2.7.6)
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do python b.py >/dev/null ; i=$(($i-1)); done )
```

## Run Python (3.4.0)
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do python3 b3.py >/dev/null ; i=$(($i-1)); done )
```

## Run Ruby (1.9.3)
```sh
time ( i=3000 ; while [ "$i" -gt 0 ]; do ruby c.rb >/dev/null ; i=$(($i-1)); done )
```

| Language        |   total       | user      | sys       |
| --------------: | -------------:| --------: | --------: |
| PHP 5.6.14      | 1m15.000s     | 0m46.490s | 0m18.40s  |
| Python 2.7.9    | 0m30.221s     | 0m14.78s  | 0m5.74s   |
| Python 3.4.2    | 0m46.814s     | 0m31.77s  | 0m6.02s   |
| Ruby 2.1.5      | 1m15.17s      | 0m57.76s  | 0m8.08s   |

