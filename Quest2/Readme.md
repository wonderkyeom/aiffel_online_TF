# AIFFEL Campus Online 4th Code Peer Review Templete
- 코더 : 김경민
- 리뷰어 : 나융


# PRT(PeerReviewTemplate)
- [x] **1.코드가 정상적으로 동작하고 주어진 문제를 해결했나요?**
```
# 현재 player는  2 번 유저입니다.
# 나온 주사위 값은  6 입니다.
# 이동 전  2 번 플레이어의 위치는  96 입니다.
# 이동 후 player들의 위치는 다음과 같습니다.
# 1 번 플레이어의 위치는 22 입니다.
# 2 번 플레이어의 위치는 102 입니다.
# 2 번 플레이어가 게임에서 승리하셨습니다.
```
> 문제 상황을 잘 정의해서 원하는 결과로 마무리하는 과정이 보였
음

</br>

- [ ] **2.주석을 보고 작성자의 코드가 이해되었나요?**
```python
if str(i) in pipe.keys():
        # + value만큼
        goal[idx-1] = pipe[str(i)]
    elif str(i) in snake.keys():
        # - value만큼
        goal[idx-1] = snake[str(i)]
    else:
        goal[idx-1] += i
```
> 간단한 주석들이라 어떤의미인지 다시 해석해야했음


</br>


- [x] **3.코드가 에러를 유발할 가능성이 있나요?**
```python
pipe = {'4':16, '8':12, '18':38, '20':74, '24':36, '32':56, '40':60, '48':54, '70':88, '76':86, '80':100, '90':92}
snake = {'22':2, '28':6, '30':10, '44':26, '58':42, '66':14, '68':52, '72':50, '84':62, '94':64, '96':82, '98':78}
```
```python
if str(i) in pipe.keys():
        # + value만큼
        goal[idx-1] = pipe[str(i)]
    elif str(i) in snake.keys():
        # - value만큼
        goal[idx-1] = snake[str(i)]
    else:
        goal[idx-1] += i
```
> 선수의 위치를 다루는 데이터 형을 str, int 로 다루고 있어 입출력단에서 에러를 발생시킬 수 있을 것 같습니다
 

</br>

- [x] **4.코드 작성자가 코드를 제대로 이해하고 작성했나요?**
```python

# 현재 player는  2 번 유저입니다.
# 나온 주사위 값은  6 입니다.
# 이동 전  2 번 플레이어의 위치는  96 입니다.
# 이동 후 player들의 위치는 다음과 같습니다.
# 1 번 플레이어의 위치는 22 입니다.
# 2 번 플레이어의 위치는 102 입니다.
# 2 번 플레이어가 게임에서 승리하셨습니다.
```
> 빠르게 문제상황을 정의하고, 최소한의 기능만 추가해서 구현한 부분이 좋았습니다


</br>

- [x] **5.코드가 간결한가요?**
```python
i = random.randint(1, 6)
    print("나온 주사위 값은 ", i, "입니다.")
    print("이동 전 ", idx, "번 플레이어의 위치는 ", goal[idx-1],"입니다.")
```
> 변수들이 들어갈 위치를 확실하고 직관적으로 표기해주어, 코드를 파악하기 편리했음


</br>


# 참고 링크 및 코드 개선
```python
# 코드 리뷰 시 참고한 링크가 있다면 링크와 간략한 설명을 첨부합니다.
# 코드 리뷰를 통해 개선한 코드가 있다면 코드와 간략한 설명을 첨부합니다.
```
