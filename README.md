# kdeepfashion_RecSys

### Original git
- https://github.com/ahmedrashed-ml/GraphRec


### Build Docker Image
```
# 도커이미지 빌드
sudo docker build -t graphrec:v1 .
# 생성된 도커이미지 확인
sudo docker images
```

```
# 생성된 도커이미지 실행
sudo docker run graphrec:v1
```
- Result
<table>
    <thead>
        <tr>
            <td>result</td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><img src="https://github.com/hyunyongPark/kdeepfashion_RecSys/blob/main/img/result.PNG"/></td>
        </tr>
    </tbody>
</table>


### Requirements
```
# python version : 3.8.13
pip install -r requirements.txt 
```



### cmd running

The install cmd is:
```
conda create -n your_prjname python=3.8
conda activate your_prjname
cd {The virtual environment directory that you created}
pip install -r requirements.txt
```
- your_prjname : 생성할 가상환경 이름


### 학습 weight file 다운로드 
아래의 링크를 통해 학습 weight 파일을 다운받습니다. 
해당 파일은 kdeepfashion 데이터셋을 학습한 trained file입니다.
해당 weight 파일은 "./model_kfashion_add_externel" 에 위치하도록 합니다.  
- https://drive.google.com/drive/folders/1tm6HLIx_r9jNquIUPyGtHk1TQR2XOWIw?usp=sharing

<table>
    <thead>
        <tr>
            <td>Example</td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><img src="https://github.com/hyunyongPark/removal_code/blob/main/img/img1.PNG"/></td>
        </tr>
    </tbody>
</table>


The testing cmd is: 
```

python3 rembg/src/rembg/cmd/cli.py --input_path "원본 이미지가 저장된 로컬 경로" --output_path "배경제거 처리 된 이미지가 저장될 경로"

```



### Result
<table>
    <thead>
        <tr>
            <td>training Plot</td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><img src="https://github.com/hyunyongPark/kdeepfashion_RecSys/blob/main/model_kfashion_add_externel/training_result.png"/></td>
        </tr>
    </tbody>
</table>




### References

- https://www.ismll.uni-hildesheim.de/pub/pdfs/Ahmed_RecSys19.pdf
- https://github.com/ahmedrashed-ml/GraphRec
- https://arxiv.org/abs/2204.06519

