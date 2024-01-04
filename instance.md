**<성능 측정>**
*cpu 사용량과 memory 사용량* 


  ```python
  import os
  import psutil


  def _check_usage_of_cpu_and_memory():

    pid = os.getpid()
    py  = psutil.Process(pid)

    cpu_usage   = os.popen("ps aux | grep " + str(pid) + " | grep -v grep | awk '{print $3}'").read()
    cpu_usage   = cpu_usage.replace("\n","")

    memory_usage  = round(py.memory_info()[0] /2.**30, 2)

    print("cpu usage\t\t:", cpu_usage, "%")
    print("memory usage\t\t:", memory_usage, "%")
```
---
**<인스턴스 유형_(T 계열 인스턴스 크기 변경)>**
<br>
- t4g.nano
<br>
<img width="411" alt="KakaoTalk_Photo_2024-01-04-16-34-14 001" src="https://github.com/eunxoo/eunxoo/assets/80334038/1970076d-916a-4680-bc0e-b0b5540e64e5">
<br>

- t4g.micro
<br>
<img width="394" alt="KakaoTalk_Photo_2024-01-04-16-34-14 002" src="https://github.com/eunxoo/eunxoo/assets/80334038/2cb5ad68-4ded-44a9-9369-dc3fe095a17e">
<br>

- t4g.small
<br>
<img width="510" alt="KakaoTalk_Photo_2024-01-04-16-34-14 003" src="https://github.com/eunxoo/eunxoo/assets/80334038/abda38cc-859e-4ee1-9f2a-938a27de1014">


---
**<구현 페이지>**
<br>
<img width="516" alt="KakaoTalk_Photo_2024-01-04-16-41-51" src="https://github.com/eunxoo/eunxoo/assets/80334038/2d0e582c-d109-41e4-b659-ecee6ed2d45e">


