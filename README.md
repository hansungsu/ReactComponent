# 컴포넌트 작업 가이드

## 필요한 컴포넌트 구현체(headlessUI 참고)

- DropMenu
- Disclosure -> 아코디언 : 숨겨진 것을 보여주는 UI
- Dialog -> 모달 팝업
- Popover -> 텍스트 위에 뜨는 말풍선
- Tabs
- Transition ? 왜 트렌지션이 headless ui 로 필요한지?
- Button
- Checkbox
- Combobox -> select 박스와 select안에 들어있는 내용 검색을 제공
- Fieldset -> input, select, textarea 등 ? 왜 input 과 나뉘어져 있는지?
- Input
- ListBox -> select
- Textarea
- Select -> 진짜 Select ? 2개를 나누는 이유는 ?
- RadioGroup
- Switch

## 이 외에 추가적인 Component들 (Shadcn 참고)

- Date Picker
- Carousel
- Chart
- Table
- Drawer - 밑에서 위로 올라오는 팝업창? 모달창?
- Navigation Menu - 마우스 on 시 나오는 메뉴그룹?
- Resizable - 마우스 드래그로 화면의 영역을 움직일 수 있음
- Scroll Area -기본 스크롤이 아닌 스크롤 디자인
- Sheet - 우측에서 나오는 레이어 팝업 모달
- Sidebar - 클릭하면 작은버전 클릭하면 큰버전
- Skeleton
- Slider - 볼륨저절기
- Toggle - switch 와 같은 느낌

## 컴포넌트에 들어가야 하는 기능들

- 키보드 탐색 (Tab, 화살표 키)
- ESC 키로 닫기
- 클릭 외부 감지
- ARIA 속성 자동 설정
- 포커스 관리
- 상태 관리 간소화:
- active, disabled 등의 상태를 자동으로 관리
- 컴포넌트 간의 상태 동기화
- 애니메이션 처리:
- enter/leave 상태에 따른 자연스러운 전환
- DOM에서 완전히 제거되기 전 애니메이션 완료 보장
- 접근성:
- 스크린리더 지원
- WAI-ARIA 패턴 준수
