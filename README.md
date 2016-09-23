# P3 pooling

- what's P3?
    - text color image format
    - please see https://en.wikipedia.org/wiki/Netpbm_format
- what's pooling?
    - aka mosaic

```
Usage: pooling [options]
    -s, --size [int]                 default=2
        --max                        max pooling (default)
        --min                        min pooling
        --avg                        avg pooling
```

## max pooling

```bash
pooling --size 10 --max < ./org.ppm > max.ppm
```

![](resources/max.png)

## avg pooling

```bash
pooling --size 10 --avg < ./org.ppm > avg.ppm
```

![](resources/avg.png)

## min pooling

```bash
pooling --size 10 --min < ./org.ppm > min.ppm
```

![](resources/min.png)


# image convert to P3 format

with Imagemagick

```bash
convert -compress none < input.ppm > output.ppm
```

