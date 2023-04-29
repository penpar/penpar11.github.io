# Stock Viewer
본 프로젝트는 React와 React Bootstrap을 이용하여, 주식 종목 검색 및 주식 정보를 조회할 수 있는 웹 어플리케이션입니다.

## 구현된 기능
주식 종목 검색 기능(자동완성)
선택한 주식의 정보 조회 기능

## 사용한 패키지
- react
- react-dom
- react-bootstrap
- react-bootstrap-typeahead
- papaparse
- axios
- dotenv

## 파일 구성
- components/HeaderNavbar.js: 상단 네비게이션 컴포넌트입니다.
- components/SearchBar.js: 주식 종목을 검색할 수 있는 검색바 컴포넌트입니다.
- components/StockViewer.js: 주식 정보를 보여주는 컴포넌트입니다.
- utils/GetStockInfo.js: API를 이용하여 주식 정보를 가져오는 함수입니다.
- App.js: 메인 어플리케이션 컴포넌트입니다.
- data/stocks.csv: 주식 종목 정보가 담긴 파일로 자동완성 기능 구현에 사용됩니다.
- 
## 주요 구현 내용
### SearchBar.js
- csv 파일에서 주식 종목 정보로 자동완성 기능을 구현하였습니다.
- `react-bootstrap-typeahead`을 이용하여 검색 기능을 구현하였습니다.
- "Clear" 버튼을 클릭하면 검색어가 초기화되도록 하였습니다.
### StockViewer.js
- 선택한 주식의 주식 정보를 가져와서 `react-bootstrap`의 `Card`로 디자인하여 보여주도록 하였습니다.
### GetStockInfo.js
- `공공데이터포털(www.data.go.kr)` API를 호출하여 주식 정보를 가져오는 함수입니다.
- `axios` 패키지를 이용하여 API 호출을 구현하였습니다.
- API 호출 시 필요한 인자들을 .env 파일에서 관리하도록 하였습니다.
### App.js 
- `react-router-dom`을 이용하여 구현하였습니다.

## 데모 페이지
[penpar.github.io](https://penpar.github.io/)

## License

This project is licensed under the MIT License.
