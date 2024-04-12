# Weekly Report

# Update: 2023/12/22 US Time
## What I have done
- Read paper [MEDITAB](https://arxiv.org/pdf/2305.12081.pdf)
- Read paper [TransTab](https://arxiv.org/pdf/2205.09328.pdf)
## TODO
- Read code of [TransTab](https://arxiv.org/pdf/2205.09328.pdf)
- Reproduce [TransTab](https://arxiv.org/pdf/2205.09328.pdf) (Deadline: 2024/01/07 US Time)

# Update: 2024/01/06 US Time
## What I have done
- Read code of [MEDITAB](https://arxiv.org/pdf/2305.12081.pdf)
- Read code of [TransTab](https://arxiv.org/pdf/2205.09328.pdf)

## TODO
- Reproduce [MEDITAB](https://arxiv.org/pdf/2305.12081.pdf) (Deadline: 2024/01/18 US Time)
- Reproduce [TransTab](https://arxiv.org/pdf/2205.09328.pdf) (Deadline: 2024/01/18 US Time)

# Update: 2024/03/26 US Time
- I was having fever last week, I will catch up the progress next week
---
# Update: 2024/04/10 US Time
- I was trying to solve the bug "can't launch tensorboard" when launching jupyter notebook [SOLVED, I change the version of image to 19.09 pytorch]
- I was trying to launch jupyter notebook and open in my pc. It is running without error on server, but the link can't be opened in my pc. [still debugging]
```
jupyter notebook --ip 0.0.0.0 --no-browser --allow-root --port 7790 --notebook-dir notebooks/ &
```
```
 To access the notebook, open this file in a browser:
        file:///root/.local/share/jupyter/runtime/nbserver-626-open.html
    Or copy and paste one of these URLs:
        http://hostname:8888/?token=XXX
     or http://127.0.0.1:7791/?token=XXX
```
I tried the following method to forward this to my pc via running the following in my pc.
```
ssh -N -f -L localhost:8888:rzhuang@129.106.31.45:7791 rzhuang@129.106.31.39
```
it returns
```
rzhuang@129.106.31.39's password: 
bind [127.0.0.1]:8888: Address already in use
channel_setup_fwd_listener_tcpip: cannot listen to port: 8888
Could not request local forwarding.
```
