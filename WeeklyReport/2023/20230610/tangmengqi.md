
# 周报
## 本周：
原本计划把省赛题补一补，但这周三lx突然和我说要出题，就先出题了，这次题出的有点急，也没沟通的太好，抓的题没有梯度，导致4个小时有点坐牢。
这周六做了一天的每日一题，刚开始做还好，越做脑子越乱，越想不明白，感觉思维还是不行，好几次想了半天没想出来最后只与题解差了一步之遥。
这次的G题头一次用逆元交上去了，做了三次逆元了，终于有一次能交上去纪念一下：
```c++
inline int cc(int n,int m) {
	int sum = 1;
	int k = 1;
	if (m==0) {
		return 1;
	}
	for (int i = n;i>=n-m+1;--i) {
		sum = (sum * i) % mod;
	}
	for (int i = 1;i<=m;++i) {
		k = (k * i) % mod;
	}
	return (sum * inv(k, mod))%mod;
}
```
这周的比赛开题开了一道我自己认为挺简单的题，结果做了两个小时，做到最后才发现可以离散化，但再改已经太晚了，就硬着头用三个for交了一下结果能过。
补了一道省赛题，省赛题出的确实好，各种算法套在一起用，代码也不长，出题人确实厉害。
## 下周:
继续补一补省赛的题，再练一练思维。