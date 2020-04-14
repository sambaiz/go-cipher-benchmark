## go-cipher-benchrmark

[Goのcipher packageに実装されている暗号利用モードのベンチマーク - sambaiz-net](https://www.sambaiz.net/article/268/)

```
$ make bench
goos: darwin
goarch: amd64
BenchmarkShortEncryptWithCBC-4                    852924              1323 ns/op             416 B/op          6 allocs/op
BenchmarkShortDecryptWithCBC-4                   1000000              1045 ns/op             240 B/op          4 allocs/op
BenchmarkShortEncryptWithCFB-4                   1213734               987 ns/op             240 B/op          4 allocs/op
BenchmarkShortDecryptWithCFB-4                   1228692              1155 ns/op             240 B/op          4 allocs/op
BenchmarkShortEncryptDecryptWithOFB-4             701252              1608 ns/op             736 B/op          4 allocs/op
BenchmarkShortEncryptDecryptWithCTR-4             709312              1747 ns/op             736 B/op          4 allocs/op
BenchmarkLongEncryptWithCBC-4                      60972             23010 ns/op           27264 B/op          6 allocs/op
BenchmarkLongDecryptWithCBC-4                      54586             22122 ns/op           13680 B/op          4 allocs/op
BenchmarkLongEncryptWithCFB-4                      34948             30435 ns/op           13680 B/op          4 allocs/op
BenchmarkLongDecryptWithCFB-4                      38904             28475 ns/op           13680 B/op          4 allocs/op
BenchmarkLongEncryptDecryptWithOFB-4               59216             20488 ns/op           14176 B/op          4 allocs/op
BenchmarkLongEncryptDecryptWithCTR-4               50810             23594 ns/op           14176 B/op          4 allocs/op
```

