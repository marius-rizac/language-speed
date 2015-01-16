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

| Language        |   read        | user      | sys       |
| --------------: | -------------:| --------: | --------: |
| PHP 5.5.9       | 1m52.333s     | 1m14.740s | 0m36.947s |
| Python 2.7      | 0m40.247s     | 0m27.252s | 0m13.178s |
| Python 3.4      | 1m6.288s      | 0m53.569s | 0m12.576s |
| Ruby 1.9.3      | 0m41.135s     | 0m27.719s | 0m9.803s  |

