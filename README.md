# movieScoreVisual
영화 평점 데이터 분석 &amp; 시각화

목표
- 무료로 공개된 영화 데이터셋을 불러와서
  - 장르별 평균 평점 계산
  - 연도별 제작 영화 수 변화
  - 인기 감독 상위 5명 찾기
- 결과를 그래프와 표로 시각화
- Python + Pandas + Matplotlib/Seaborn 사용
---

데이터셋
- 출처: TMDB 5000 Movie Dataset (Kaggle)
- 크기: 약 5000개의 영화 정보
- 주요 컬럼:
  - title (영화 제목)
  - release_date (개봉일)
  - vote_average (평점)
  - vote_count (투표 수)
  - genres (장르 JSON 문자열)
  - director (감독)
---

구체적인 진행 단계
1. 환경 준비
  - Python 3.12.2
  - Jupyter Notebook 설치
2. 데이터 불러오기
  - Kaggle에서 데이터 다운로드 후 tmdb_5000_movies.csv 저장
  - Pandas로 CSV 읽기
3. 데이터 전처리
  - 결측치 제거
  - 장르 문자열을 실제 리스트로 변환
  - 개봉년도 추출 (연도별 분석 위해)
4. 데이터 분석
  - 장르별 평균 평점
  - 연도별 영화 제작 수 변화
  - 평점 상위 10개 영화
  - 투표 수가 많고 평점이 높은 감독 TOP 5
5. 시각화
  - 장르별 평균 평점 막대그래프
  - 연도별 영화 제작 수 꺾은선 그래프
  - 감독 TOP 5 바 차트
6. 결과 저장
  - 그래프를 PNG로 저장
  - 분석 리포트를 .ipynb와 .html로 저장