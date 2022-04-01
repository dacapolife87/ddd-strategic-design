# 키친포스

## 요구 사항

### 상품

- 상품을 등록할 수 있다.
- 상품의 가격이 올바르지 않으면 등록할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 이름이 올바르지 않으면 등록할 수 없다.
    - 상품의 이름에는 비속어가 포함될 수 없다.
- 상품의 가격을 변경할 수 있다.
- 상품의 가격이 올바르지 않으면 변경할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 가격이 변경될 때 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 크면 메뉴가 숨겨진다.
- 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

- 메뉴 그룹을 등록할 수 있다.
- 메뉴 그룹의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴 그룹의 이름은 비워 둘 수 없다.
- 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

- 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
- 상품이 없으면 등록할 수 없다.
- 메뉴에 속한 상품의 수량은 0 이상이어야 한다.
- 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴는 특정 메뉴 그룹에 속해야 한다.
- 메뉴의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 이름에는 비속어가 포함될 수 없다.
- 메뉴의 가격을 변경할 수 있다.
- 메뉴의 가격이 올바르지 않으면 변경할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴를 노출할 수 있다.
- 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 높을 경우 메뉴를 노출할 수 없다.
- 메뉴를 숨길 수 있다.
- 메뉴의 목록을 조회할 수 있다.

### 주문 테이블

- 주문 테이블을 등록할 수 있다.
- 주문 테이블의 이름이 올바르지 않으면 등록할 수 없다.
    - 주문 테이블의 이름은 비워 둘 수 없다.
- 빈 테이블을 해지할 수 있다.
- 빈 테이블로 설정할 수 있다.
- 완료되지 않은 주문이 있는 주문 테이블은 빈 테이블로 설정할 수 없다.
- 방문한 손님 수를 변경할 수 있다.
- 방문한 손님 수가 올바르지 않으면 변경할 수 없다.
    - 방문한 손님 수는 0 이상이어야 한다.
- 빈 테이블은 방문한 손님 수를 변경할 수 없다.
- 주문 테이블의 목록을 조회할 수 있다.

### 주문

- 1개 이상의 등록된 메뉴로 배달 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 포장 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 매장 주문을 등록할 수 있다.
- 주문 유형이 올바르지 않으면 등록할 수 없다.
- 메뉴가 없으면 등록할 수 없다.
- 매장 주문은 주문 항목의 수량이 0 미만일 수 있다.
- 매장 주문을 제외한 주문의 경우 주문 항목의 수량은 0 이상이어야 한다.
- 배달 주소가 올바르지 않으면 배달 주문을 등록할 수 없다.
    - 배달 주소는 비워 둘 수 없다.
- 빈 테이블에는 매장 주문을 등록할 수 없다.
- 숨겨진 메뉴는 주문할 수 없다.
- 주문한 메뉴의 가격은 실제 메뉴 가격과 일치해야 한다.
- 주문을 접수한다.
- 접수 대기 중인 주문만 접수할 수 있다.
- 배달 주문을 접수되면 배달 대행사를 호출한다.
- 주문을 서빙한다.
- 접수된 주문만 서빙할 수 있다.
- 주문을 배달한다.
- 배달 주문만 배달할 수 있다.
- 서빙된 주문만 배달할 수 있다.
- 주문을 배달 완료한다.
- 배달 중인 주문만 배달 완료할 수 있다.
- 주문을 완료한다.
- 배달 주문의 경우 배달 완료된 주문만 완료할 수 있다.
- 포장 및 매장 주문의 경우 서빙된 주문만 완료할 수 있다.
- 주문 테이블의 모든 매장 주문이 완료되면 빈 테이블로 설정한다.
- 완료되지 않은 매장 주문이 있는 주문 테이블은 빈 테이블로 설정하지 않는다.
- 주문 목록을 조회할 수 있다.

## 용어 사전

### 메뉴그룹
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 메뉴그룹 | menu group | 메뉴의 묶음으로 하나 이상의 메뉴를 포함한다 |

### 메뉴
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 메뉴 | menu |  한 개 이상의 상품으로 구성된 손님이 주문하는 주문 단위이며 특정 메뉴 그룹에 속함 |
| 메뉴 노출 상태 |  menu display status | 메뉴가 고객에서 노출되는지 상태여부 |
| 메뉴 노출 | menu display | 메뉴를 고객에서 노출시킨다. |
| 메뉴 숨김 | menu hide | 메뉴를 숨긴다. |

### 상품
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 상품 | product | 이름과 가격을 갖고 있으며 메뉴에 포함될 수 있는 제품을 뜻한다 |
| 상품 가격 | product price | 상품의 가격 |
| 상품 수량 | product quantity | 상품의 갯수 |

### 주문테이블
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 테이블 | order table | 매장에서 손님들이 주문하는 테이블 |
| 주문 테이블 착석 | order table sit | 주문테이블에 손님들이 착석한 상태 |
| 주문 테이블 착석여부 | order table status | 주문테이블이 사람이 착석되어있는지 판단하는 상태 |
| 주문 테이블 손님 수 | order table number Of guests | 주문테이블에 착석되어 있는 사람 수 |
| 빈 테이블 | empty table | 주문 테이블이 비어있는 상태 |

### 주문
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 | order | 고객이 상품을 요청하는 행위 |
| 주문 타입 | order type | 주문의 유형(매장주문, 포장주문, 배달주문 의 유형이 존재한다.) |
| 배달 주소 | delivery address | 배달주문을 수령하는 장소 |
| 주문 상태 | order status | 주문의 진행 상태 (대기, 접수, 서빙, 배달시작, 배달완료, 완료 의 상태가 존재한다.)  |
| 키친라이더 | kitchen rider | 배달을 해주는 사람 |
| 배달 요청 | delivery request | 배달주문이 접수될 경우 키친라이더에게 배달을 요청한 상태 |

### 주문 타입 (주문의유형)
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 매장주문 | eat in order | 매장에서 식사하는 주문 타입 |
| 포장주문 | take out order | 상품을 포장하는 주문 타입 |
| 배달주문 | delivery order | 상품을 배달요청하는 주문 타입 |

### 주문상태 (주문의 진행 상태)
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 대기 | order waiting | 주문이 요청된 상태 |
| 접수 | order accept | 판매자가 주문을 확인하여 접수한 상태 |
| 서빙 | order serve | 요청된 주문이 준비된 상태 |
| 배달시작 | delivery start | 배달주문이 배달을 시작한 상태 |
| 배달완료 | delivery complete | 배달주문이 완료된 상태 |
| 완료 | order complete | 요청된 주문의 모든과정이 완료된 상태 |

### 공통
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 비속어 | profanity word | 격이 낮고 속된 말 |

## 모델링

New
### 상품
- 상품(Product)은 이름(name), 가격(price)을 가진다.
- 상품(Product)의 이름(name)에는 비속어(Profanity)가 포함될수 없다.

- 상품(Product)을 등록(create)한다.
  - 상품(Product)의 가격(price)은 0원 이상이어야 한다.
  - 상품(Product)의 이름(name)에는 비속어(Profanity)가 포함될수 없다.
- 상품(Product)의 가격(price)을 변경(change)할 수 있다.
  - 상품(Product)의 가격(price)이 변경될때 메뉴(Menu)의 가격(price)이 메뉴에 속한 상품(MenuProduct) 금액의 합(sum)보다 크면 메뉴가 숨겨진다.(hide)
- 상품(Product)의 목록을 조회(findAll)할수 있다.

### 메뉴그룹
- 메뉴그룹(MenuGroup)은 이름(name)을 가진다

- 메뉴그룹(MenuGroup)을 등록(create)한다.
  - 메뉴그룹(MenuGroup)의 이름(name)은 비워둘 수 없다.
- 메뉴그룹(MenuGroup)의 목록을 조회(findAll)한다.

### 메뉴
- 메뉴(Menu)는 이름(name), 가격(price)을 가진다
- 메뉴(Menu)는 하나이상의 메뉴상품(MenuProduct)을 가진다. 
- 메뉴(Menu)는 하나의 메뉴그룹(MenuGroup)에 속한다.
- 메뉴(Menu)는 노출상태여부(displayed)를 가진다.
  
- 메뉴(Menu)를 등록(create)한다.
  - 메뉴(Menu)의 가격(price)은 0원 이상이어야한다.
  - 메뉴(Menu)는 추가할 메뉴 그룹(MenuGroup)이 있어야 한다.
  - 메뉴의 이름(name)에는 비속어(Profanity)가 포함될수 없다.
  - 메뉴(Menu)의 가격은 메뉴상품(MenuProduct)들의 가격의 합보다 작아야한다.
- 메뉴(Menu)의 가격을 변경(change)한다.
  - 메뉴(Menu)의 가격은 메뉴상품(MenuProduct)들의 가격의 합보다 작아야한다.
- 메뉴(Menu)를 노출(display)한다.
  - 메뉴(Menu)의 가격이 메뉴상품(MenuProduct)들의 가격의 합보다 클경우 노출할수 없다.
- 메뉴(Menu)를 미노출(hide) 한다.
- 메뉴(Menu)의 목록을 조회(findAll)한다.
  

### 주문테이블
- 주문테이블(OrderTable)은 이름(name)을 가진다.
- 주문테이블(OrderTable)은 0명 이상의 손님수(numberOfGuests)를 가진다.

- 주문테이블(OrderTable)을 등록(create)한다.
  - 주문테이블(OrderTable)의 이름(name)은 비워둘수 없다.
- 주문테이블(OrderTable)을 착석(sit)한다.
- 주문테이블(OrderTable)을 정리(clear)한다.
  - 주문테이블(OrderTable)의 주문중 완료(complete)되지 않은 주문(Order)이 있을경우 변경할수 없다.
- 주문테이블(OrderTable)의 손님수(numberOfGuests)를 변경(change)한다.
  - 주문테이블(OrderTable)이 빈테이블(empty) 일 경우 손님수(numberOfGuests)를 변경할 수 없다.
- 주문테이블(OrderTable)의 목록을 조회(findAll)한다.

### 주문
- 주문(Order)은 주문유형을(type)을 가진다.
  - 주문유형(OrderType)은 배달주문(deliveryOrder), 포장주문(takeOutOrder), 매장주문(eatInOrder)이 있다.
- 주문(Order)은 주문상태(status)를 가진다.
  - 주문상태(status)는 대기(waiting), 접수(accept), 서빙(serve), 배달시작(delivery start), 배달완료(delivery complete), 완료(complete) 가 있다.

- 주문(Order)을 등록(create)한다.
  - 주문(Order)시 주문유형(type)은 필수이다
  - 주문(Order)시 주문아이템(OrderLineItem)은 존재해야한다.
  - 미노출(hide)된 메뉴(Menu)는 주문할수 없다.
  - 메뉴(Menu)의 가격(price)과 주문(Order)의 가격(price)이 다르면 불가능하다
  - 매장주문(eatInOrder)이 아닐경우 주문아이템(OrderLineItem)의 수량(quantity)은 0이상이어야 한다.
  - 배달주문(deliveryOrder)은 배송지(deliveryAddress)정보가 필수이다
  - 매장주문(eatInOrder)의 경우 주문테이블(OrderTable)이 존재해야한다.
- 주문(Order)을 접수(accept)한다.
  - 대기(waiting)중인 주문(Order)만 접수(accept)할 수있다.
  - 배달주문(deliveryOrder)이 접수(accept)되면 배달 대행사(kitchen rider)를 호출(delivery request)한다.
- 주문(Order)을 서빙(serve)한다.
  - 접수(accept)된 주문(Order)만 서빙(serve)할 수 있다.
- 주문(Order)을 배달(delivery)한다.
  - 배달주문(deliveryOrder)만 배달(delivery start)할 수 있다.
  - 서빙(serve)된 주문(Order)만 배달(delivery start)할 수 있다.
- 주문(Order)을 배달완료(delivery complete) 한다.
  - 배달(delivery start)중인 주문(Order)만 배달완료(delivery complete)할 수 있다.
- 주문(Order)을 완료(complete)한다.
  - 배달주문(deliveryOrder)의 경우 배달완료(delivery complete)된 주문(Order)만 완료(complete)할 수 있다.
  - 포장(takeOut Order) 및 매장 주문(eatInOrder)의 경우 서빙(serve)된 주문(Order)만 완료(complete)할 수 있다.
  - 주문테이블(OrderTable)의 모든 주문(Order)이 완료(complete)되면 빈테이블(empty)로 정리(clear)한다.
- 주문(Order)목록을 조회(findAll)한다.

