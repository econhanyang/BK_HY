<h1> 주거환경 만족도 영향요인 분석</h1>
<h2> :직방 아파트 리뷰 데이터와 BERT 모형을 활용하여 </h2>
<h6> 텍스트기반 경제사회 빅데이터 분석 <br><br>
    도시공학과 2022249754 권준현

본 연구는 직방의 **아파트 리뷰 데이터**를 수집하고 딥러닝 기반의 자연어 처리 모형인 **BERT**와 기계학습 방법론인**SHAPley Value** 등을 활용하여 주거환경 만족도의 영향요인을 분석하였다. 구체적으로는 아파트 리뷰의 내용을 바탕으로 주거환경 만족도의 긍정적, 부정적 영향 요인을 도출하고 서울 시 내 권역별로 나타나는 차이를 비교하였으며, 이들의 연관어를 도출해 주거환경 만족도 개선을 위한 주요 사항을 제시하였다.
<h3>'주거환경'이란?</h3>
<h6>  주거와 생활 장소를 둘러싸고 있는 생활환경의 총체로, 물리적 환경 및 사회적, 경제적, 문화적 환경을 모두 포함하는 개념 (아사미 야스시, 2003) </h6>
<h3>'주거환경 만족도'란?</h3> <h6>  사람들이 주관적으로 체험하는 주거환경 만족도는 사회적, 물리적 환경에 대한 정서적인 반응으로, 거주 가능성과 도시의 지속가능성 등을 판단하는 주요한 지표로 작용함 (신은진·남진, 2012; 안용진, 2016)  </h6>
<h3>'아파트'는?</h3> <h6>  아파트는 주거생활의 총체적 경험을 제공하며, 가장 보편적인 주거형태임 (이유재·문선희, 2016) </h6> <h6> 최근 온라인 서비스를 통해 아파트를 포함한 다양한 부동산 유형에 대한 정보를 쉽게 확인 가능하며, 더 나아가 웹 크롤링, 텍스트 마이닝을 통해 주거환경 만족도의 영향요인 분석, 부동산 임대료 예측 모형 개발 등이 가능 (김보찬 외, 2018; 김선재·이수기, 2020)</h6>
<h2><p style="color:orange">본 연구는?</p></h2>
<h3> <span style ="background-color:yellow"> 아파트 리뷰 빅데이터를 활용해 주거환경 만족도 영향요인을 분석함</span> </h3>
<br>


<i>설문조사로 구축한 정량적인 자료만을 활용, 조사자가 정한 항목만을 고려, 수동적으로 주거환경 만족도의 영향요인을 도출한 기존 연구와 딜리 본 연구는 다음과 같은 차별성을 지님</i>
    
<b>① 서울특별시 전체 아파트를 대상으로 주거환경 만족도를 수집

<b>② 딥러닝 자연어처리 모델 활용, 만족도의 긍정적, 부정적 영향요인 자동 추출

<b>③ 서울특별시 다섯 개 권역*에 따른 주거환경 만족도 영향요인 도출 및 분석
<h2>본 연구의 프레임워크 </h2>

![image](https://user-images.githubusercontent.com/131750990/234494435-23b0b76a-d3c1-4cc9-895a-40bf00d3e76a.png)


  
<텍스트리뷰 전처리 예시>
  
![image](https://user-images.githubusercontent.com/131750990/234492066-99a672e5-78c3-4574-b00d-884213b1139e.png)
    
  
<BERT 활용 방법>
![image](https://user-images.githubusercontent.com/131750990/234492118-e0f80741-7cea-4611-944c-e6300b7f618a.png)
<Shap 활용 예시>![image](https://user-images.githubusercontent.com/131750990/234492221-334d61c8-f382-404c-a0ac-b9d264c91bc6.png)
<h2><p style="color:red">주요결과요약</p></h2>
아래 그림은 각 권역별로 도출된 영향요인 중 긍정적/부정적 영향요인에 대해 상위 5개 요인과 이를 바탕으로 도출한 주요 주제를 나타낸 것임

![image](https://user-images.githubusercontent.com/131750990/234492324-f9a76a4a-c373-4ea2-b26f-cdc13855ac93.png)
다음 그림은 각 권역에서 한 번이라도 도출된 상위 영향요인들에 대해, 서울 전체 리뷰에 대한 상대적 영향력과 연관어를 시각화한 것임

![image](https://user-images.githubusercontent.com/131750990/234492397-cd97ef8b-a1ca-4b3e-a730-b7ce05b9bcf4.png)
<h3>연구 결론</h3>

- 첫째, 서울 전체적으로 아파트의 경제적 가치가 주거환경 만족도에 영향을 미침
- 둘째, 도출된 주거환경 만족도 영향요인을 고려하여 권역별 다른 계획 수립이 가능
- 셋째, 아파트 리뷰를 활용한 인프라 요소 및 사람들 관심사의 모니터링이 가능
<h3>향후 진행 방향</h3>

- 한글 언어 전처리 정교화(인터넷 용어, 오탈자, 어간 정규화 등에서 오는 오류 등)
- 한글에 적합한 BERT 모형 토크나이저 검증 및 적용
- 리뷰 작성자의 개인적 특성 및 공간 단위의 규모 고려 
- 리뷰 작성 시점 구분하여 분석(데이터 편향 고려)
