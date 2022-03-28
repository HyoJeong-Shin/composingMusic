## children's song dataset 구하기

1. audioset에서 eval_segments.csv 다운로드   
2. class_labels_indices.csv에서 children's song에 해당하는 장르 코드를 찾은 후   
3. eval_segments.csv에서 그 코드에 해당하는 데이터만 분류   
4. youtube-dl을 통해 dataset 다운로드   
<br>

```python
# youtube-dl install
!pip install youtube-dl

# mp3 format으로 다운로드
!youtube-dl -x --audio-format mp3 <youtube link>
```
<br>


- mp3 → music sheet 변형 소프트웨어   [AnthemScore](https://www.youtube.com/watch?v=Vqfv_vrnt1Y)
    - 동요들 mp3들은 가사가 존재하여 잘 인식될 지 모르겠음 😞
    - 우선 되는지 시도 해보려면 **AnthemScore and MuseScore3 소프트웨어 구매 필요**  
