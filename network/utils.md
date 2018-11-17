## 1. Get mac address

```
  # First ping to ip address
  ping <ip-address>
  
  # Show mac address of ping history
  arp -a 
```

## 2. Trace ip route

```
  traceroute 8.8.8.8
```

## 3. Find external ip

```
  curl ipinfo.io/ip
```

## 4. List open ports

```
  # Localhost
  sudo netstat -tulpn

  # Remote 
  sudo nmap -O remote_host
```

## 5. Check port is open

```
  nc -zv <host> <port>
```

## 6. List all ip connect to port

```
netstat -tn 2>/dev/null | grep :<port> | awk '{print $5}' | cut -d: -f1 | sort | uniq -c | sort -nr | head
```

## 7. Speed test

```
http://makezine.com/projects/send-ticket-isp-when-your-internet-drops/
```




