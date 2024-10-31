## Pisano 周期

2<sub>n+2</sub> = b * u<sub>n+1</sub> + c * u<sub>n</sub>

```python
#sage
g = 17665922529512695488143524113273224470194093921285273353477875204196603230641896039854934719468650093602325707751568
mod = 100000007
R = BinaryRecurrenceSequence(6,1)
#计算序列的周期
cycle = R.period(mod)
print(R(g%cycle)%mod)

#output :41322239
```
