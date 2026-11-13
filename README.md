# 토우이야기

신라 토우를 사진과 자료로 살펴보는 온라인 웹 전시입니다. 사진 위에 마우스를 올리거나 모바일에서 사진을 터치하면 원형 돋보기로 세부 모습을 확인할 수 있습니다. 마지막 전시에서는 국가유산청의 통일신라 인물 토우 파편을 페이지 안에서 직접 돌려볼 수 있습니다.

## GitHub Pages로 공개하기

1. GitHub에서 새 저장소를 만들고, 이 폴더 안의 `index.html`, `README.md`, `.nojekyll`, `assets` 폴더를 저장소 최상위에 올립니다.
2. 저장소의 **Settings → Pages**로 이동합니다.
3. **Build and deployment**의 Source를 **Deploy from a branch**로 설정합니다.
4. Branch는 `main`, 폴더는 `/ (root)`를 선택하고 저장합니다.
5. 잠시 후 Pages 설정 화면에 표시되는 주소에서 전시를 확인합니다.

ZIP을 사용한다면 압축을 먼저 풀고, 압축 파일 자체가 아니라 안에 들어 있는 파일과 `assets` 폴더를 저장소에 올리세요.

## 파일 구성

- `index.html` — 전시 페이지와 3D 뷰어
- `assets/` — 토우 사진, 출토 지점 사진, 3D 모델과 텍스처
- `.nojekyll` — GitHub Pages가 정적 파일을 그대로 제공하도록 하는 설정 파일

## 전시 내용과 출처

전시는 사진에서 관찰되는 모습과 박물관 자료에 기록된 내용을 구분해 소개합니다. 개별 토우의 출토지가 확인되지 않은 경우 임의로 지역을 붙이지 않습니다. 노래·춤은 사용자 제공 사진에서 받은 인상으로 표현하고, 개체의 정식 명칭이나 출토 정보는 확인된 것처럼 단정하지 않습니다.

- [참고글: 신라 토우 이야기](https://irona.tistory.com/62)
- [국립중앙박물관 K759 소장품 정보](https://www.museum.go.kr/MUSEUM/contents/M0502000000.do?relicId=2659&schM=view&searchId=search)
- [국립중앙박물관 토우 큐레이터 추천](https://www.museum.go.kr/MUSEUM/contents/M0501000000.do?pageSize=10&relicRecommendCategory=&relicRecommendId=166326&sc=&schM=view&sv=)
- [국립경주박물관 토우장식 항아리](https://gyeongju.museum.go.kr/site/kor/html/sub04/0402.html?dvs_code=c020110&mng_no=42&mode=V)
- [국가유산 디지털 서비스: 개모양 토우](https://digital.khs.go.kr/buis/buisDetail.do?bizUid=13930741327849003132)
- [공공데이터포털: 국가유산청 서라벌 천년왕경 토우편 3D 에셋](https://www.data.go.kr/data/15165336/fileData.do)

## 3D 자료

국가유산청 「서라벌 천년왕경 토우편」 FBX/PNG 서비스본으로 회전형 뷰어를 구성했습니다. 이 모델은 통일신라 인물 토우 파편으로, 앞서 소개한 K760·K759·K895와는 다른 개체입니다. 국가유산청은 목과 얼굴이 결실되고 몸통·어깨·팔다리 일부가 남았다고 설명합니다. 뷰어는 Three.js FBXLoader와 OrbitControls를 사용하며, 라이브러리는 CDN에서 불러옵니다. 모델은 공공누리 제1유형(출처표시) 조건으로 제공됩니다.