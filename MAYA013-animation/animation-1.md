# Animation
## Key 찍기 전 setting
1. locator 위치 시키기
   * create>locator
   * 스냅 걸어서 이동
1. 큐브, 컨트롤러(Create>NURBS primitives) 만들기
1. 큐브, 컨트롤러 함께 선택하고 v를 눌러서 locator와 겹치게 위치시키기
   * x는 그리드 스냅, v는 vertex 스냅
   * 다하면 freeze, delete history
1. 큐브 선택, 컨트롤러 선택, P
   * 회전용, 이동용 컨트롤러가 따로있었다면 orient와 point를 따로했겠지만, 지금은 그럴 필요가 없기 때문에 그냥 P
1. locator 선택, 컨트롤러 선택, CP
1. 큐브의 크기를 적절히 맞추고 freeze
   * Parent는 자식이 독단적으로 행동할 수 있기 때문에 큐브 크기를 수정한 후 다시 freeze를 누를 수 있다는 장점이 있다
  
1. locator 선택, Hand  선택, P
   * 공이 기계와 함께 움직여야 하니까.
  


## Key 찍는법
   * S버튼을 눌러 찍을 수 있다.
   * 지우려면 원하는 프레임에 두고 오른쪽버튼 > delete
   * 수정하려면, 원하는 프레임에 두고 수정한다음 다시 S버튼
   * 키는 부모만 찍힌다.
   
   frame|1|29|30|52|60|61|90|120|150|180|181|200|250
   ---|---|---|---|---|---|---|---|---|---|---|---|---|---
   Hand_CTR|v| |v| |v| |v|v|v| | |v|v
   Ball_CTR| | | | |v|v| | | |v|v| | 
   U_H_CTR| |v| |v|v| | |v|v| | |v|v
   
1. Ball 컨트롤러 선택 후 60 프레임에 키를 찍는다
    * Blend Parent가 0 &rarr; key값을 따라간다.
    * Blend Parent가 1 &rarr; CP를 따라간다.
    * Blend Parent에 키가 안찍혔으면 S두번
1. Blend Parent 0 60
1. Blend Parent 1 61

