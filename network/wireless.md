## 1. iwgetid

Get information or wireless network

```
iwgetid [interface] [--raw] [--scheme] [--ap] [--freq]
                      [--mode] [--protocol] [--channel]
```


```Shell
$ iwgetid 
```

## 2. iwlist

Scan network

```Shell
$ sudo iwlist wlan0 scan | grep ESSID
```