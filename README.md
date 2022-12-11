# 이미지 인식을 통한 타투 분류<br>
<br>

## 0. 목차
<table>
    <thead>
        <tr align=center>
            <th>번호</th>
            <th>목차</th>   
        </tr>
    </thead>
    <tbody>
        <tr align=center>
            <td>1</td>
            <td><a href="#1">Subject</a></td>
        </tr>
        <tr align=center>
            <td>2</td>
            <td><a href="#2">Data</a></td>
        </tr>
        <tr align=center>
            <td>3</td>
            <td><a href="#3">Model</a></td>
        </tr>
        <tr align=center>
            <td>4</td>
            <td><a href="#4">Summary</a></td>
        </tr>
        <tr align=center>
            <td>5</td>
            <td><a href="#5">Result</a></td>
        </tr>
     </tbody>
</table>
<br>

## 1.<a name="1">Subject</a>  
- 타투 입문자들이 늘어나는 반면 얻을 수 있는 정보에 대한 접근이 제한적  
- 이미지 인식을 통한 타투 스타일 분류  
- 입문자도 접근이 용이한 타투 플랫폼 구축

## 2.<a name="2">Data</a>

![스크린샷_20221211_120719](https://user-images.githubusercontent.com/113493695/206884446-cd4e2b1e-0950-4228-b0ea-624ad55e66a0.png)

## 3.<a name="3">Model</a>

![스크린샷_20221211_120934](https://user-images.githubusercontent.com/113493695/206884486-4eb0d943-a8ff-4648-8865-95115cf6f872.png)

- ILSVRC 대회 역대 우승 알고리즘에서 모델을 선택

<table>
    <thead>
        <tr align=center>
            <th><a href="#alexnet">AlexNet</a></th>
            <th><a href="#vgg">VGG 16 / 19</a></th>
            <th><a href="#resnet50">ResNet50</a></th>
            <th><a href="#resnet152">ResNet152</a></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>- Data Augmentation<br>- Dense Change</td>
            <td>- Transfer Learning<br>- Dense Change<br>- ReduceLROnPlateau</td>
            <td>- Transfer Learning<br>- Dense Change<br>- ReduceLROnPlateau</td>
            <td>- Transfer Learning<br>- Resize(300x300)</td>
        </tr>
    </tbody>
</table>
<br>

### <a name="alexnet">AlexNet</a>

![스크린샷_20221211_122138](https://user-images.githubusercontent.com/113493695/206884753-7a4cb363-d3c1-4d5a-871c-aa248a5f3511.png)

![스크린샷_20221211_122207](https://user-images.githubusercontent.com/113493695/206884768-caf24d86-a5d9-4ab8-88cd-74df786e6003.png)

### <a name="vgg">VGG 16/19</a>

![스크린샷_20221211_122530](https://user-images.githubusercontent.com/113493695/206884869-873d4098-885a-44a5-b917-169a23ce9e3e.png)

![스크린샷_20221211_122555](https://user-images.githubusercontent.com/113493695/206884880-f9e2782c-31a5-49a7-a902-e768b9424cdc.png)

![스크린샷_20221211_122631](https://user-images.githubusercontent.com/113493695/206884890-0251e049-e00c-4cc4-8ad8-1d5d30da6f4e.png)

### <a name="resnet50">ResNet50</a>

![스크린샷_20221211_123027](https://user-images.githubusercontent.com/113493695/206884975-42cd4858-1a2a-4a5e-bc66-e4d167396b36.png)

![스크린샷_20221211_123059](https://user-images.githubusercontent.com/113493695/206884992-b6301681-0dc3-498a-82a6-217ba68b1923.png)

![스크린샷_20221211_123134](https://user-images.githubusercontent.com/113493695/206885011-9b475122-7c39-4501-9ceb-dd13338f5b13.png)

### <a name="resnet152">ResNet152</a>

![스크린샷_20221211_123311](https://user-images.githubusercontent.com/113493695/206885048-f9b5907e-3ed8-4641-b849-0ee782ab8598.png)

![스크린샷_20221211_123342](https://user-images.githubusercontent.com/113493695/206885059-ca0569a1-9b55-484e-9efa-dd58e6c4968d.png)

![스크린샷_20221211_123425](https://user-images.githubusercontent.com/113493695/206885075-4a5e1772-cd2c-42bc-b6ad-3bf3f795f9ea.png)

## 4.<a name="4">Summary</a>
### Compare

![스크린샷_20221211_123755](https://user-images.githubusercontent.com/113493695/206885155-4bcfa097-bdc6-4515-bb87-2d1a00c2d488.png)

<table>
    <thead>
        <tr align=center>
            <th>Model</th>
            <th>Val_Accuracy</th>   
        </tr>
    </thead>
    <tbody>
        <tr align=center>
            <td>CNN</td>
            <td>0.2869</td>
        </tr>
        <tr align=center>
            <td>AlexNet</td>
            <td>0.6799</td>
        </tr>
        <tr align=center>
            <td>VGG 16</td>
            <td>0.7602</td>
        </tr>
        <tr align=center>
            <td>VGG 19</td>
            <td>0.7923</td>
        </tr>
        <tr align=center>
            <td>ResNet50</td>
            <td>0.7987</td>
        </tr>
        <tr align=center>
            <td>ResNet152</td>
            <td>0.8474</td>
        </tr>
    </tbody>
</table>
<br>

## 5.<a name="5">Result</a><br>(Market Positioning)

![스크린샷_20221211_124720](https://user-images.githubusercontent.com/113493695/206885388-46da20f4-3123-440e-a451-8525f81be7e6.png)

### 고객의 시선

![스크린샷_20221211_124754](https://user-images.githubusercontent.com/113493695/206885410-8843cf5a-f06a-4d82-b4de-22ff1d445f50.png)

### 타투이스트의 시선

![스크린샷_20221211_124841](https://user-images.githubusercontent.com/113493695/206885421-e6791e08-5c8a-4240-b60c-f307e292bc0e.png)
