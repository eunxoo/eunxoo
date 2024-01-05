## **<테스트 코드>**
*실행 시간* 


  ```python
def logging_time(original_fn):
    import time
    from functools import wraps

    @wraps(original_fn)
    def wrapper(*args, **kwargs):
        start_time = time.time()
        result = original_fn(*args, **kwargs)

        end_time = time.time()
        print("WorkingTime[{}]: {} sec".format(original_fn.__name__, end_time - start_time))
        return result
    return wrapper
```
---
## **<인스턴스 유형_(T 계열 인스턴스 크기 변경)>**
<br>


### t4g.nano
- 평균 시간 : 21.60408


<img width="693" alt="KakaoTalk_Photo_2024-01-05-08-46-31" src="https://github.com/eunxoo/eunxoo/assets/80334038/437c1a8c-bba9-4ac0-8edd-d150cc64b091">

<br>
<br>

### t4g.micro
- 평균 시간 : 21.51994


<img width="700" alt="KakaoTalk_Photo_2024-01-05-08-47-14" src="https://github.com/eunxoo/eunxoo/assets/80334038/9499d607-16ae-4b5b-9549-600316adff52">

<br>
<br>

### t4g.small
- 평균 시간 : 21.18853

<img width="694" alt="KakaoTalk_Photo_2024-01-05-08-47-35" src="https://github.com/eunxoo/eunxoo/assets/80334038/4682fce9-67f2-411f-9976-135943d99208">

<br>


<img width="830" alt="스크린샷 2024-01-05 오전 9 30 53" src="https://github.com/eunxoo/eunxoo/assets/80334038/4af583d2-e4ad-49b8-ac8d-59929af1e60f">

---
## **<구현 페이지>**
<br>
<img width="516" alt="KakaoTalk_Photo_2024-01-04-16-41-51" src="https://github.com/eunxoo/eunxoo/assets/80334038/2d0e582c-d109-41e4-b659-ecee6ed2d45e">


