# 유튜브 뉴스 댓글 분석을 통한 ChatGPT 여론조사 : 감성분석과 네트워크 분석을 중심으로
- ChatGPT에 관련된 뉴스 댓글을 크롤링한 뒤, 감성분석과 네트워크 분석을 수행하여 ChatGPT에 관련된 긍정/부정적인 감정의 원인을 알아보는 연구
- 2024-1 국어정보학 기말개인연구 결과물입니다.

## 구조
- youtube_crawling.ipynb : 유튜브 댓글 크롤링
- crawling_data_cleansing.ipynb : 유튜브 댓글 데이터 정제
- sentiment_analysis.ipynb : 감성 분석 모델 개발 및 유튜브 댓글 대상 예측
- corpus_analysis : 유튜브 댓글 데이터 형태소 분석, 빈도 분석, 네트워크 모델링을 위한 파일 생성
- data : 분석에 활용되는 데이터를 보관하는 폴더
    - model : 감성분석에 활용되는 데이터를 보관하는 폴더
    - network : 네트워크 분석에 활용되는 데이터를 보관하는 폴더
    - tokenize : 형태소 분석에 활용되는 데이터를 보관하는 폴더
    - youtube_chatgpt_news_comments.csv : 유튜브 댓글 크롤링 수행 직후의 원시 말뭉치
    - youtube_chatgpt_news_comments_cleaned.csv : 데이터 정제를 수행한 말뭉치
    - youtube_chatgpt_news_comments_with_sentiment.csv : 감성 분석을 수행하여 긍정적인 댓글은 1, 부정적인 댓글은 0으로 라벨링된 말뭉치

## 유의사항
- youtube_crawling.ipynb는 jupyter notebook, 이외 코드는 colab 환경에서 실행
- 환경에 따라 별도의 파일 경로 설정 필요