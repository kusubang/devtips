# Code Snippets

## Mac

- convert []byte to string

```go
mac := []byte{1, 1, 1, 1, 1, 1}
a := net.HardwareAddr(mac)
fmt.Println(a)
// result: 01:01:01:01:01:01
```
