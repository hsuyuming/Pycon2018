### Python efficency
profiling
Cython
asyncio

### backend 
https://imgur.com/a/KfBrqZJ
Slow API :
CPU :
Harakiri : Ling request process termination (uwsgi Harakiri)


### What's asyncio
https://imgur.com/a/a0oaXXM
make io conchronous

Asynchronous I/O
Running I/O cocurrently

Blocking IO mode

Aync IO mode

小孩像ＣＰＵ 大人像ＩＯ

### asyncio as solusion
API runs faster and user get better experiment.

### Myths about asyncio
https://imgur.com/a/0ch76GX

python 3.6.5 開始可以使用aync
```python 
async def sleep_and_return(sec):
    await asyncio.sleep(sec)
    return sec

sleep_and_return()
<coroutine object sleep_and_return >

run async function in event loop

asyncio.get_event_loop().rin_util_complete(sleep_and_return(1))
```

### How asyncio works?
https://imgur.com/a/Q5YJKWa

### asyncio in instagram
https://imgur.com/a/6paFuiv
scale:collaboration in large code repo with a lot of developers
usability:asyncio untility and bug fix
prioritization: too much blocking calls to migrate

### Backend client library asyncio support
https://imgur.com/a/fikZ3BN
Thrift
Http
Other backend

### Make ayncio easier
https://imgur.com/a/ROhb3uJ
pytest 不支援async 必須用@ayncio......

### Async stack migration


### Identify blocking calls (Blocking call Finder)
collect latency/call count -> prioritize 

### Dependency
https://imgur.com/a/Kn2UC7J

### Sync 
func = sync(async_func)
https://imgur.com/a/kYE8xmU

### Runtime error1
https://imgur.com/a/Ejiv9gM

### Runtime error3 : event loop stopped before future complete
因為有可能在root的node還沒改成aync
https://imgur.com/a/n71lAAE

### Global variable issue
https://imgur.com/a/jtGlwXv

### Gather design pattern
https://imgur.com/a/vJN9I4x

### LINT -> code rule
https://imgur.com/a/zs2Ywyt

### Automation
https://imgur.com/a/IgsuWv3

### CPU OVERHEAD
CPU problem aync use python not cpython
https://imgur.com/a/x8Ezrgq

### CUSTOM OPTIMIZATION
https://imgur.com/a/4fCDRi3

### Current results
API latency become 30% faster on server side
https://imgur.com/a/4vjhuKC

### Q&A

Django not have aync -> Answer copy that and add more function


### ref 
1.https://instagram-engineering.com/