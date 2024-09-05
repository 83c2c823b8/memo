```sh
printf "%s\n" x y z "w"
x
y
z
w
```

```sh
printf "%5s\n" "x  y"  "y----z"
    x
    y
```

```sh
printf "%-5s\n" "x  y"  "y                z"
```

```sh
printf "%*s\n" 5 x 3 y
    x
  y
```
