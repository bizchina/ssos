####常用的一些命令：

get，set （常见的数据存储）

哈希（用于大量的数组集合的存储，占用内存更小，但是存储的数据字节应该尽量的小）：
hset($key, $field, $value)
hget($key, $field)

zadd ($key, $score, $value)（可以根据score用于对数据的排序，计数等等）
zcard
zrange
zrevrange (排序，避免数据库的排序，加快效率)

####redis优化
1.将数字字符串转成整型将减少存储大小