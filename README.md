# _rand 随机数生成

## 安装

```go
go get -u github.com/koyeo/_rand
```

## 随机数生成

> 注意：
> `_randInt*` 方法要求 max 大于0

```go
_rand.Int(0, 1)         // 生成 [0,1] 之间的随机数
_rand.Int32(-1, 1)      // 生成 [-1,1] 之间的随机数
_rand.Int64(-100, 100)  // 生成 [-100,100] 之间的随机数
```

## 验证码生成

```go
_rand.Code(4)    // 生成4位由 [1,9] 数字组成的验证码
```