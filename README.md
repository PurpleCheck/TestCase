# ZeroError Test Case
## Step1) Scan Inspect ID
![1000000000001](https://user-images.githubusercontent.com/51939302/186175852-acec0a51-f3f4-4d1e-854e-74c00809ba32.png)

### Success
* 상품 검수 화면으로 전환된다.
* 검수할 주문 상품 목록이 생성된다.

### Fail
* 비정상 검수 바코드 -> 존재하지 않는 검수 바코드 오류 안내가 노출된다.
* 검수 완료 바코드 -> 이미 검수가 완료된 바코드 오류 안내가 노출된다.
* 검수 바코드 스캔 화면이 유지된다.


## Step 2) Scan Item ID
![그린티 퓨어 젤 핸드크림](https://user-images.githubusercontent.com/51939302/186175945-c7d12299-5d2b-408f-bb20-d9a2c5a0a7e2.png)   
그린티 퓨어 젤 핸드크림 x2   
   
![스틱레브르 오리지널](https://user-images.githubusercontent.com/51939302/186176068-3a672809-0342-4555-9ab2-8e5492a9f0bc.png)   
스틱레브르 오리지널 x2   
   
![엔젤스코튼 너리싱 핸드크림](https://user-images.githubusercontent.com/51939302/186176230-509c3031-4404-49f6-873c-b1fcb7a2fbb6.png)   
엔젤스코튼 너리싱 핸드크림 x2   
   
### Success
* 상품 바코드 스캔이 완료 될때마다 달성율이 증가한다. (Bar & Count)
* 상품 바코드 스캔이 완료 되면 상품 목록(ORDER LIST)에 해당 상품의 검수 Count가 증가한다.
* 주문 갯수 만큼 검수가 끝난 상품은 상품 목록에서 보라 -> 회색으로 변경된다.
* 주문한 상품의 스캔이 모두 완료되면 송장 바코드 스캔 화면으로 전환된다.

### Fail
* 주문 내역에 없는 상품 경고창을 노출한다.   
예 -> 검수 바코드 스캔 화면으로 전환된다.   
아니요 -> 상품 바코드 스캔화면이 유지된다.


## Step 3) Scan Tracking ID
![T100000000001](https://user-images.githubusercontent.com/51939302/186176301-007abc47-94c7-4efc-a35c-3bde42a84cdf.png)

### Success
* 검수 완료 알림창이 노출된다.
* 검수 바코드 스캔 화면으로 전환된다.

### Fail
* 송장번호 불일치 오류 안내가 노출된다.
