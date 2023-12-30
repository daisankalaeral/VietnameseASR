# Dataset

```
VSDB_train.json
{
    "ex0": {
        "wav": "36688.wav",
        "class": "[0F0NY]",
        "text": "Đến lúc nhận được thì chỉ có nhận được có ba triệu rưỡi",
        "duration": 2.5405,
        "editedby": "B21DCCN497"
    },
    "ex1": {
        "wav": "25937.wav",
        "class": "[0M0NY]",
        "text": "Thay mặt ủy ban kiểm tra trung ương ông Trần Cẩm Tú chủ nhiệm ủy ban kiểm tra trung ương tiếp thu ý kiến chỉ đạo của đồng chí trưởng đoàn kiểm tra",
        "duration": 6.335687,
        "editedby": "B21DCCN599"
    },
    "ex2": {
        "wav": "02432.wav",
        "class": "[ phát biểu , nam , nam , 50, nghiêm túc]",
        "text": "ngay từ kì họp thứ hai  ủy an thường vụ quốc hội đã thống nhất với chính phủ về chủ trương và tích cực chỉ đạo chuẩn bị nội dung",
        "duration": 9.046062,
        "editedby": "B21DCVT013"
    }
}
```
Download the dataset from [here](https://drive.google.com/drive/folders/1tiPKaIOC7bt6isv5qFqf61O_2jFK8ZOI)

# Training

## Transformer
```
cd transformer_asr
python transformer_words_train.py hparams/Transformer.yaml
```
## Transformer with  SpecAugmentation
```
cd transformer_asr
python transformer_words_train.py hparams/Transformer_SpecAugment.yaml
```
## Transformer with Adaptive SpecAugmentation
```
cd transformer_asr
python transformer_words_train.py hparams/Transformer_AdaptiveSpecAugment.yaml
```
## LAS
```
cd las_asr
python las_train.py hparams/LAS.yaml
```
## LAS with SpecAugmentation
```
cd las_asr
python las_train.py hparams/LAS_SpecAugment.yaml
```
