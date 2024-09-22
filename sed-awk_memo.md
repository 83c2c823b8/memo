# printf
```sh
printf "%s\n" x y z "w"
x
y
z
w
```

```sh
printf "%10s\n" "x  y"  "y----z"
      x  y
    y----z
```

- left alignment
```sh
printf "%-10s\n" "x  y"  "y----z"
x  y
y----z
```

```sh
printf "%*s\n" 5 x 3 y
    x
  y
```

# sed
```sh
seq 10 | awk '{print $1%5$}' | sed -n '/2/,/4/p'
```
2にマッチする行から4にマッチする行
```sh
seq 10 | awk '{print $1%5$}' | awk '/2/,/4/p'
```
awk も同様

```sh
echo a | sed -r 's/./\0/' 
```
\0 は見つけた文字列全体
