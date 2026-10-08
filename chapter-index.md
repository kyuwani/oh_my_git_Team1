# Index
## 1. Step by Step
```bash
git checkout "step-by-step"
echo "A smoke detector. It's now going off!" > smoke_detector
git commit -am "Now alarm go off!"
```

## 2. Add new files to the index
```bash
# 세미콜론을 통해 한 줄로 실행 시 1번 조건이 달성되지 않음.(버그)
git add candle
git commit -am "Add the candle"
```

## 3. Update files in the index
```bash
echo "Now melting..." >> candle
git add candle
git commit -am "Make a commit"
```

## 4. Reseting files in the index
```bash
# add하지 않으면 1번 조건이 달성되지 않음.
git add red_candle
git reset blue_candle green_candle
# -am으로 커밋 시, red_candle 이외도 함께 커밋되기 때문에 2번 조건을 달성할 수 없음.
git commit -m "make a commit!"
```

## 5. Adding changes step by step
```bash
# 1번 조건: 모든 파일에 수정사항을 주기
echo But now sugar in the water. >> bottle
echo Hammer hit the sugar cube. >> hammer
echo Broken sugar cube has putted to the bottle.

# 2번 조건: 아무 파일 하나를 add하기
git add hammer

# 3번 조건: 커밋하기
git commit -m "Hammer hit the sugar cube!!"

# 4번 조건: 하나의 파일만 변경한 커밋을 하기.
git add sugar_cube; git commit -m "put broken sugar cube to the bottle."

# 5번 조건: 마지막 남은 파일도 커밋하기.
git add bottle; git commit -m "Now sugar in the water in the bottle."
```