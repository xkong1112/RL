# CPU没办法自动降频

```bash
sudo apt install i7z#查看CPU频率，全满就是不知道降频的那种
sudo i7z
sudo apt install cpufrequtils
sudo vim /etc/default/grub
GRUB_CMDLINE_LINUX="splash quiet"
GRUB_CMDLINE_LINUX_DEFAULT="intel_pstate=disable"
sudo update-grub
```

# 称砝码

```python
 def getWeight(n,weight,num):
    res = {0}
    for i in range(n):
        temp = res.copy()
        for j in range(1,num[i]+1):
            for k in temp:
                res.add(k + weight[i]*j)
    return len(res)
 
while True:
    try:
        n = int(input())
        weight = list(map(int,input().split()))
        num = list(map(int,input().split()))
        print(getWeight(n,weight,num))
    except:
        break
```

