## 1.	HPE ProLiant DL360 Gen10 Model
- 고성능과 보안을 자랑하는 고밀도 1U 랙 서버.

  ※ProLiant : 서버 브랜드 이름
    DL : 고밀도 서버 (360 : 1U / 2개의 CPU),(380 : 2U / 2개의 CPU)
    Gen10 : 10세대 모델

  1) 프로세서 소켓 : 듀얼 소켓을 지원하여 최대 28코어의 인텔, 제온 스케일러블 프로세서를 장착할 수 있다.
  2) 메모리 슬롯 : 최대 24개의 DDR4 DIMM슬롯을 제공하여 최대 3TB 메모리를 지원한다.
  3) 스토리지 인터페이스 : NVMe, SAS, SATA 인터페이스를 지원하여 다양한 스토리지 옵션을 제공. NVMe > SAS > SATA
  4) 확장 슬롯 : 최대 3개의 PCle 3.0슬롯을 제공하여 추가적인 확장 카드를 장착할 수 있다.
 
※ DL360 과 DL380의 차이점 
- DL360 : 1U, 1개 Riser에 2개의 NIC 및 구성품 삽입 가능, 기본 디스크8개 + 후면 드라이브에 2개 추가가능 
- DL380 : 2U, 1개 Riser에 3개의 NIC 및 구성품 삽입 가능, 기본디스크 24개+ 후면 드라이브에 6개 추가가능 

### **2U Riser NIC Slot**

![image](https://github.com/user-attachments/assets/9d46a4a9-d100-4f84-a751-914210720ac0)


### **DL 380 plus PCle slot**

![image](https://github.com/user-attachments/assets/4ba84d66-5e0a-41d8-9dc9-1059fc4b2d97)
 



### SAS와 SATA
![SATA 와 SAS](https://github.com/user-attachments/assets/a408d6bc-7a53-40de-b812-c41d51a47bc2)


### HPE ProLiant DL360 Gen10 Model (1U)
![HPE ProLiant DL360 Gen10 (1U)](https://github.com/user-attachments/assets/cc2d7776-946c-44eb-b4bc-4261e2fa56b2)


### HPE ProLiant DL380 Gen10 Model (2U)
![HPE ProLiant DL380 Gen10 Model (2U)](https://github.com/user-attachments/assets/cb8b15b0-5594-4403-8343-bdcde09b3bb3)

---

2.	RAM 부착 순서
- 1) 메모리 채널 확인 : 메모리 슬롯은 흰색과 검은색으로 구분. 흰색 슬롯이 메모리 채널의 시작점, 검은색 슬롯이 두 번째 슬롯.
  2) CPU별 슬롯 : 각 CPU는 12개의 DIMM 슬롯을 제어한다. 따라서 듀얼 CPU 구성에는 총 24개의 DIMM슬롯을 사용할 수 있다.(총2개CPU)
  3) 메모리 모듈 설치 : 메모리 모듈을 설치할 때는 흰색 슬롯부터 시작하여 검은색 슬롯 순서로 설치. 모듈을 올바른 방향으로 삽입하고, 완전히 장착되었는지 확인
  4) 속도 및 용량 : CPU에 따라 지원되는 메모리 속도와 용량이 다르다.

### 메모리 슬롯

![메모리 슬롯](https://github.com/user-attachments/assets/9681a8ee-9b41-41ac-ad01-01638e0e0ac8)


### RAM DIMM 
![RAM DIMM](https://github.com/user-attachments/assets/47ed884a-cedf-41a2-b011-3d36642b9f50)


![DIMM](https://github.com/user-attachments/assets/cbf0412c-6f96-468e-88df-37a0f1c9935c)

---
3.	CPU 부착 방법
- 1) CPU 소켓 준비 : CPU 소켓의 보호 커버를 제거하고, 소켓 레버를 들어 올려 소켓을 연다.
  2) CPU 설치 : CPU를 소켓에 맞춰서 조심스럽게 놓는다. **CPU의 핀이 손상되지 않도록 주의** **CPU의 삼각형 마크와 소켓의 삼각형 마크를 맞춰 설치**(순서는 CPU 슬롯위 나사 고정순서 기입되어있음.)
  3) 방열판 부착 : 방열판을 CPU 위에 놓고, 방열판의 나사를 조여서 단단히 고정. (방열판위 나사 고정 순서 기입되어있음.)

### CPU 슬롯 
![CPU 슬롯](https://github.com/user-attachments/assets/5cff10ce-d251-4f70-8fd3-29a544825edb)

### 방열판 
![방열판](https://github.com/user-attachments/assets/bc34a826-15f7-497f-b945-24c8c05845cb)

4.	서버 내 부품 설명(Raid Controller, Cooler, SSD, HDD, OCP, NIC)
  1) Raid Controller

  ![Controller](https://github.com/user-attachments/assets/4f069bcd-2f7e-4555-a9a3-51998bc42f4e)
  - 컨트롤러는 여러 개의 하드 디스크 드라이브(HDD)또는 솔리드 스테이트 드라이브(SSD)를 하나의 논리적 유닛으로 결합하여 데이터 중복성 및 성능을 향상시키는 장치.
  - RAID 레벨에 따라 데이터 보호와 성능 향상 방법이 다르다.

  2) Cooler
  
  ![Cooler](https://github.com/user-attachments/assets/5dc10fad-dcba-4f92-9e49-dfb3073c8c17)
  - 쿨러는 서버 내부의 열을 방출하여 CPU와 기타 부품이 과열되지 않도록 하는 장치. 

  3) OCP
 
  ![OCP](https://github.com/user-attachments/assets/228be02f-d7e8-4574-aad4-ff7bbe0d2e9b)
  - OCP 슬롯은 라이저 카드 내부에 위치할 수 있다.
  - OCP 슬롯은 네트워크 인터페이스 카드(NIC)와 같은 추가 하드웨어를 설치할 수 있는 확장 슬롯으로, 서버의 확장성과 유연성을 높이는 데 사용된다.

### Riser
![riser](https://github.com/user-attachments/assets/5a1c8c78-d134-479e-bdc9-da0a7d869640)


5.	전력 W(와트)별 파워 설치 방법 
  - 서버의 전력 요구 사항에 따라 적절한 전원 공급 장치를 선택.
  ex) 500W, 800W, 1600W등 전원 공급 장치가 있다. 보통 500W, 800W를 많이 쓴다. 
6.	CPU code 
  - ex) CPU뒷면에 code : 4210 silver / Gen10 = DELL 14세대

        4 : silver
        5,6 : Gold
        8 : Platinum 등급을 뜻함.

        1,2 Gen10 = DELL 14세대
        3   Gen10plus = DELL 15세대
        4,5 Gen11 = DELL 16세대
7.	서버 랙 레일킷 설치 방법
- 1) 타워에 부착된 레일에 서버를 끼워 놓는방법
   Gen9 및 이전 모델에서 사용
  2) 타워에서 레일을 분리해, 분리된 레일에 서버를 끼워서 타워에 설치하는 방법 
   Gen10 및 이후 모델에서 사용 


