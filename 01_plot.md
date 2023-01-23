### [1] 선 그래프

**`plot()`** 함수는 직선 또는 꺾은선 형태의 그래프를 그릴 때 사용할 수 있는 명령어다.

```python
import matplotlib.pyplot as plt
plt.plot([10,20,30,40])
plt.show()	# 그래프 보여주기
```

>![다운로드](assets/01_%EA%B8%B0%EB%B3%B8%20%EA%B7%B8%EB%9E%98%ED%94%84%20%EA%B7%B8%EB%A6%AC%EA%B8%B0/%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C-16413585949351.png)

입력한 리스트의 값은 y축 값으로 입력되며, x축 값은 자동으로 0.0부터 0.5씩 증가하는 실수로 입력된다.



```python
import matplotlib.pyplot as plt
plt.plot([1,2,3,4],[12,43,25,15])
plt.show()
```

>![다운로드 (1)](assets/01_%EA%B8%B0%EB%B3%B8%20%EA%B7%B8%EB%9E%98%ED%94%84%20%EA%B7%B8%EB%A6%AC%EA%B8%B0/%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C%20(1)-16413586055502.png)

**`plot()`** 함수에 입력된 두 개의 리스트 중, **<u>첫 번째 리스트가 x 축 값</u>**이고, **<u>두 번째 리스트가 y축 값</u>**으로 입력된다.

---



### [2] 그래프에 기본적 옵션 추가하기

```python
## fontdict 파라미터
(font1=)fontdict={'family': 'serif', 'color': 'b', 'weight': 'bold', 'size': 14}
(font2=)fontdict={'family': 'fantasy', 'color': 'deeppink', 'weight': 'normal', 'size': 'xx-large'}
등등

`fontdict=~~`을 작성하거나 `fontdict=font1` 과 같이 사용할 수 있다.

fontdict 파라미터를 사용하여 각 옵션에 폰트 스타일을 적용할 수 있다.
아래에 설명할 옵션들 중 폰트 스타일 적용이 가능한 옵션이라면 [F] 라는 표시를 해둔다.
-----------------------------------------------------------------------------------------

## loc 파라미터
loc='right/left/center/top/bottom/upper left 등등'
loc='best' : 최적의 위치로 지정

loc 파라미터를 사용하여 각 옵션에 위치를 지정해준다.[L] 라는 표시를 해둔다.
-----------------------------------------------------------------------------------------

## 축 레이블 설정 [F][L]
xlabel(), ylabel() 함수
xlabel(), ylabel() 함수에 문자열을 입력
plt.xlabel('X-Label')
plt.ylabel('Y-Label')
-----------------------------------------------------------------------------------------

## 제목 명칭 [F][L]
plt.title('$') 함수 추가
-----------------------------------------------------------------------------------------

## 범례 삽입 [L]
label = '$'
plt.legend() 함수 추가.
폰트 크기 지정 : fontsize = $
범례 테두리 꾸미기: frameon=bool(범례 텍스트 상자의 테두리 표시 여부), shadow=bool(텍스트 상자의 그림자 표시 여부)
-----------------------------------------------------------------------------------------

## 그래프 색상 바꾸기
color= '$'
-----------------------------------------------------------------------------------------    
## 선 모양 바꾸기
linestyle(ls) = '$'
-----------------------------------------------------------------------------------------

## 마커 모양 바꾸기
plt.plot(x,y,'g^') 'r.'등등
marker 속성을 설정하면 선 형태가 아닌 점 형태로 그래프를 그릴 수 있다.
마커 모양으로는 선,점,동그라미,삼각형,별 모양 등 여러가지가 있다.
-----------------------------------------------------------------------------------------

# 그래프 영역 채우기
fill_between() - 두 수평 방향의 곡선 사이를 채움.
fill_betweenx() - 두 수직 방방의 곡선 사이를 채움.
fill() - 다각형 영역을 채움.
-----------------------------------------------------------------------------------------

```





![set_marker_05](assets/01_%EA%B8%B0%EB%B3%B8%20%EA%B7%B8%EB%9E%98%ED%94%84%20%EA%B7%B8%EB%A6%AC%EA%B8%B0/set_marker_05.png)