# HLL_CARDINALITY

## 功能

用于计算HLL类型值的基数。

## 语法

```Haskell
HLL_CARDINALITY(hll)
```

## 参数说明

`hll`: 通过其它列或者导入数据里面的数据生成的hhl列。

## 返回值说明

bigint 类型。

## 示例
```plain text
MySQL > select HLL_CARDINALITY(uv_set) from test_uv;
+---------------------------+
| hll_cardinality(`uv_set`) |
+---------------------------+
|                         3 |
+---------------------------+
```