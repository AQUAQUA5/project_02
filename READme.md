# SKN05-2ND-4TEAM

### 📈2차 프로젝트: 전자상거래 고객 이탈 분석 및 예측 <br>
 **개발기간: 2024.10.16-10.17**

## 💻팀 소개
**팀명** 
김이박조


**팀원**

|  **김요은👩‍💻** |  **이준호👨‍💻** |  **김혜서👩‍💻** |  **박보람👩‍💻** |
|:---------:|:---------:|:---------:|:-----------:|
| @usey10 | @Lanvizu | @Hyeseo20 |  @pbr2858 |

### 1. 프로젝트 개요
<hr>
<div>
<blockquote>

<img src="https://pds.joongang.co.kr/news/component/htmlphoto_mmdata/202204/14/e41ef02b-f4f7-453c-b7fd-fa5e96707d7a.jpg">
 <br>
<br> 이커머스 시장은 폭발적인 성장 속에 경쟁이 치열해지고 있습니다. 
 <br>소비자들은 다양한 선택지를 가지고 있기 때문에, 고객 이탈은 큰 손실로 이어질 수 있습니다. 
 <br> 시장 규모가 커질수록 고객 유지의 중요성은 더욱 커지며, 이탈 예측은 이를 해결할 핵심 도구로 떠오릅니다. 
 <br> 따라서 맞춤형 서비스 제공과 충성도 유지를 위해 고객 이탈 예측은 필수적입니다.
</blockquote>
</div> 

#### 1.2. 프로젝트 소개
<blockquote>
•	이 프로젝트를 통해 데이터 기반으로 고객 이탈에 대한 분석 내용을 제공합니다.<br>
•	 고객 이탈 분석 및 예측을 통해 이탈 고객의 행동 패턴을 분석하고, 이탈 가능성이 높은 고객을 사전에 예측하고자 합니다. <br>
•	이를 통해 이탈률이 높은 변수에 대한 적절한 전략을 마련할 수 있습니다.<br>
</blockquote>


#### 1.3. 프로젝트 목표
<blockquote>

1.	고객 이탈 가능성을 조기에 감지<br>
2.	그 원인을 분석해 유용한 정보를 제공<br>
• 이를 통해 기업은 고객 유지를 위한 맞춤형 전략을 수립할 수 있으며, 고객 이탈을 줄이는 데 필요한 통찰을 얻게 됩니다.<br>
</blockquote>
<br><br> 

### 기술 스택
 <img src="https://img.shields.io/badge/python-3776AB?style=flat-square&logo=python&logoColor=white"/></a>
 <img src="https://img.shields.io/badge/streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white"/></a>
 

### 2. EDA

| ![output](./images/output.png) |![pie](./images/PIE.png) | ![bar](./images/BAR.png) | ![box](./images/BOX.png) |
|:-----------------------------------:|:-------------------------------------:|:-----------------------------------:|:-------------------------------------:|
| 변수당 고유값에 따른 이탈률 |변수당 고유값 비율 | 변수당 고유값 수 | Boxplot   |

| ![Heatmap](./images/Heatmap.png) |
|:-------------------------------------:|
| Heatmap   |

### 3. 데이터 전처리
- #### 결측값 처리 방법
<h3 style="color:#2C3E50; text-align:center; font-size: 1.2em;">📊 PowerCo 데이터셋 결측치 분석</h3>
<div style="overflow-x:auto;">
<table style="width:100%; border-collapse: collapse; margin: 15px 0; font-family: 'NanumGothic', sans-serif; font-size: 0.85em;">
    <thead>
        <tr style="background-color:#E0F2F7; color:#2C3E50;">
            <th style="padding: 7px; border: 1px solid #ddd; text-align: center;">결측<br>유무</th>
            <th style="padding: 7px; border: 1px solid #ddd; text-align: left;">칼럼명</th>
            <th style="padding: 7px; border: 1px solid #ddd; text-align: left;">의미</th>
            <th style="padding: 7px; border: 1px solid #ddd; text-align: left;">타입</th>
            <th style="padding: 7px; border: 1px solid #ddd; text-align: center;">결측치<br>비율</th>
            <th style="padding: 7px; border: 1px solid #ddd; text-align: center;">카디널리티</th>
            <th style="padding: 7px; border: 1px solid #ddd; text-align: left;">해결 방안</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd; font-weight:bold;">activity_new</td>
            <td style="padding: 5px; border: 1px solid #ddd;">회사 활동 카테고리</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; background-color:#FFEBEE;">59.30%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">4</td>
            <td style="padding: 5px; border: 1px solid #ddd;">새 카테고리</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd; font-weight:bold;">campaign_disc_ele</td>
            <td style="padding: 5px; border: 1px solid #ddd;">고객이 마지막으로 가입한 전기 캠페인 코드</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; background-color:#F8D7DA;">100.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd; color:blue;">드랍</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd; font-weight:bold;">channel_sales</td>
            <td style="padding: 5px; border: 1px solid #ddd;">영업 채널 코드</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; background-color:#FFEBEE;">26.21%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">7</td>
            <td style="padding: 5px; border: 1px solid #ddd;">새 카테고리</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">cons_12m</td>
            <td style="padding: 5px; border: 1px solid #ddd;">최근 12개월간 전기 사용량</td>
            <td style="padding: 5px; border: 1px solid #ddd;">int64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">cons_gas_12m</td>
            <td style="padding: 5px; border: 1px solid #ddd;">최근 12개월간 가스 사용량</td>
            <td style="padding: 5px; border: 1px solid #ddd;">int64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">cons_last_month</td>
            <td style="padding: 5px; border: 1px solid #ddd;">지난달 전기 사용량</td>
            <td style="padding: 5px; border: 1px solid #ddd;">int64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">date_activ</td>
            <td style="padding: 5px; border: 1px solid #ddd;">계약 활성화 날짜</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">date_end</td>
            <td style="padding: 5px; border: 1px solid #ddd;">계약 종료 등록일</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.01%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd; font-weight:bold;">date_first_activ</td>
            <td style="padding: 5px; border: 1px solid #ddd;">고객의 첫 계약 시작일</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; background-color:#F8D7DA;">78.21%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd; color:blue;">드랍</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">date_modif_prod</td>
            <td style="padding: 5px; border: 1px solid #ddd;">상품 마지막 수정일</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.98%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">date_renewal</td>
            <td style="padding: 5px; border: 1px solid #ddd;">다음 계약 갱신일</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.25%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd; font-weight:bold;">forecast_base_bill_ele</td>
            <td style="padding: 5px; border: 1px solid #ddd;">다음 달 예상 전기 요금 기준</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; background-color:#F8D7DA;">78.21%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd; color:blue;">드랍</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd; font-weight:bold;">forecast_base_bill_year</td>
            <td style="padding: 5px; border: 1px solid #ddd;">연간 예상 전기 요금 기준</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; background-color:#F8D7DA;">78.21%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd; color:blue;">드랍</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd; font-weight:bold;">forecast_bill_12m</td>
            <td style="padding: 5px; border: 1px solid #ddd;">12개월 예상 전기 요금 기준</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; background-color:#F8D7DA;">78.21%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd; color:blue;">드랍</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd; font-weight:bold;">forecast_cons</td>
            <td style="padding: 5px; border: 1px solid #ddd;">다음 달 예상 전기 사용량</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; background-color:#F8D7DA;">78.21%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd; color:blue;">드랍</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">forecast_cons_12m</td>
            <td style="padding: 5px; border: 1px solid #ddd;">다음 12개월 예상 전기 사용량</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">forecast_cons_year</td>
            <td style="padding: 5px; border: 1px solid #ddd;">연간 예상 전기 사용량</td>
            <td style="padding: 5px; border: 1px solid #ddd;">int64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">forecast_discount_energy</td>
            <td style="padding: 5px; border: 1px solid #ddd;">예상되는 반복 할인 금액</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.78%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">forecast_meter_rent_12m</td>
            <td style="padding: 5px; border: 1px solid #ddd;">다음 12개월 미터기 임대료 예상 금액</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">forecast_price_energy_p1</td>
            <td style="padding: 5px; border: 1px solid #ddd;">1구간 예상 에너지 단가</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.78%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">forecast_price_energy_p2</td>
            <td style="padding: 5px; border: 1px solid #ddd;">2구간 예상 에너지 단가</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.78%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">forecast_price_pow_p1</td>
            <td style="padding: 5px; border: 1px solid #ddd;">1구간 예상 전력 단가</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.78%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">has_gas</td>
            <td style="padding: 5px; border: 1px solid #ddd;">고객이 가스도 사용하는지 여부</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">2</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">imp_cons</td>
            <td style="padding: 5px; border: 1px solid #ddd;">현재 결제된 사용량</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">margin_gross_pow_ele</td>
            <td style="padding: 5px; border: 1px solid #ddd;">전력 가입 총 마진</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.08%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">margin_net_pow_ele</td>
            <td style="padding: 5px; border: 1px solid #ddd;">전력 가입 순마진</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.08%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">nb_prod_act</td>
            <td style="padding: 5px; border: 1px solid #ddd;">활성화된 상품 및 서비스 개수</td>
            <td style="padding: 5px; border: 1px solid #ddd;">int64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">11</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">net_margin</td>
            <td style="padding: 5px; border: 1px solid #ddd;">총 순마진</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.09%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">X</td>
            <td style="padding: 5px; border: 1px solid #ddd;">num_years_antig</td>
            <td style="padding: 5px; border: 1px solid #ddd;">고객의 가입 경과 연수</td>
            <td style="padding: 5px; border: 1px solid #ddd;">int64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.00%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">15</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">origin_up</td>
            <td style="padding: 5px; border: 1px solid #ddd;">고객이 처음 가입한 전기 캠페인 코드</td>
            <td style="padding: 5px; border: 1px solid #ddd;">object</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.54%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">5</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
        <tr>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center; color:red;">O</td>
            <td style="padding: 5px; border: 1px solid #ddd;">pow_max</td>
            <td style="padding: 5px; border: 1px solid #ddd;">가입된 최대 전력</td>
            <td style="padding: 5px; border: 1px solid #ddd;">float64</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">0.02%</td>
            <td style="padding: 5px; border: 1px solid #ddd; text-align: center;">-</td>
            <td style="padding: 5px; border: 1px solid #ddd;">-</td>
        </tr>
    </tbody>
</table>
</div>

- #### 라밸 인코더 
| 변수명 | 라벨 인코딩 후 |
|:-----------------------------------:|:-------------------------------------:|
| PreferredLoginDevice  | 0 ~ 2 |
|PreferredLoginDevice  |0 ~ 6 |
|Gender   | 0 ~ 1|
| PreferedOrderCat   |0 ~ 5 |
| MaritalStatus   |0 ~ 2 |

- #### 스케일링한 변수
|CashbackAmount |CityTier |WarehouseToHome | 
|:-----------------------------------:|:-------------------------------------:|:-----------------------------------:|
|HourSpendOnApp |NumberOfDeviceRegistered| SatisfactionScore | 
| NumberOfAddress |Complain |CouponUsed | 
| OrderCount |DaySinceLastOrder |   | 



### 4. 모델링 & 하이퍼 파라메터 튜닝

- #### 초기 성능 확인
| ![초기성능](./images/초기성능.png) | 
|:-------------------------------------:|

- #### 1차 성능 개선
| ![oversampling](./images/oversampling.png) | 
|:-------------------------------------:|
| ![smote](./images/smote.png) | 
| ![borderlinesmote](./images/borderlinesmote.png) | 

- #### 2차 성능 개선
| ![gridsearchcv](./images/gridsearchcv.png) | 
|:-------------------------------------:|

- #### 최종 모델 분석
| ![adaboost](./images/adaboost.png) |![xgboost](./images/xgboost.png) | 
|:-----------------------------------:|:-------------------------------------:|
| adaboost | xgboost |
| ![mlp](./images/mlp.png) |![catboost](./images/catboost.png) | 
| mlp | catboost |
| ![logi](./images/logi.png) |![rf](./images/rf.png) | 
|logistic regression |randomforest |
| ![dt](./images/dt.png) |![gb](./images/gb.png) | 
| decision tree |gradient boosting|

• 모델들을 비교해 봤을 떄 Tenure, Complain, CashbackAmount 총 세 변수가 중요하다고 판단 

### 5. 예측
#### 이탈률 비교
•	 Test Data 에 대한 이탈률 예측 비교 <br>
• 실제 데이터를 가지고 도출한 이탈률 : 16.29% <br>
• 예측 데이터를 가지고 도출한 이탈률 : 15.60% <br>
• 예측 데이터의 이탈률이 실제 데이터와 상당히 비슷한 확률을 보여 예측이 잘 되었다고 생각. <br>
| ![이탈률](./images/이탈률.png) |![이탈률수치](./images/이탈률수치.png) | 
|:-----------------------------------:|:-------------------------------------:|

#### Tenure, Complain, CashbackAmount 에 대한 이탈률 확인
- #### Tenure
|![ten](./images/ten.png) | 
|:-------------------------------------:|
|61개월 이상 가입했던 고객과, 0개월~1개월 의 가입기간을 가지는 고객의 이탈률이 높음. <br>
장기 가입 고객 및 신규 가입 고객이 지속적으로 이용할 수 있는 마케팅 전략이 필요하다고 판단됨.|

- #### Complain
|![com](./images/com.png) | 
|:-------------------------------------:|
|complain 을 낸 사람들의 이탈률이 높음을 알 수 있음.<br>
complain 고객의 관리 전략이 필요하다고 판단됨.|

- #### CashbackAmount
|![cash](./images/cash.png) | 
|:-------------------------------------:|
|지난달에 고객들이 얼마나 Cashback 을 받았는지에 대한 지표 <br>
지난달 캐시백을 100 달러 미만 받은 고객은 오히려 이탈률이 없었으나,<br> 100달러 단위와 비슷하게 캐시백을 받은 고객의 이탈률이 조금 존재하는 편.<br>
100 달러 단위의 할인 정책이 있지 않을까 예측<br>
고객의 캐시백 정보에 대한 데이터의 추가적인 분석이 필요하다고 판단됨.|

### 6. 결론

| **위 피처들을 통한 이탈 방지 전략을 구현을 제안** |
|:-------------------------------------:|
| 장기 가입 고객 및 신규 가입 고객 타겟의 마케팅 전략<br> 컴플레인 고객 관리 전략<br> 캐시백 정보에 대한 추가적 분석 |

### 7. Streamlit 예측 시각화

![image](https://github.com/user-attachments/assets/aefab40a-6a5a-4b59-a523-54912b0a5495)

![image](https://github.com/user-attachments/assets/a48d701a-93f0-4822-9b46-fe6982d288c4)

 
### 8. 한 줄 회고
<hr>
<blockquote>

•	김요은 : 다 같이 한 과정 한 과정 진행했음에 즐거웠고 여러 모델을 돌리면서 각 모델에 대해 더 알아보고 이해할 수 있는 좋은 시간이었습니다. <br>
•	이준호 : 체계적인 계획에 따라 진행하면서 전체적인 프로젝트의 흐름과 각각의 모델의 특징을 공부하고 적용하는 시간이라 좋았습니다. <br>
•	김혜서 : 프로젝트를 통해 데이터 분석에 대한 이해도가 높아지고 이에 대한 공부를 할 수 있는 기회였습니다 <br>
•	박보람 : 거의 모든 과정을 팀원들과 같이 나누어 진행하여 하나씩 경험할 수 있어 너무 좋았다. 프로젝트를 진행하면서 통계 지식이 부족함을 깨달았고, 기초부터 다시 공부하고 싶다는 생각을 했다.
