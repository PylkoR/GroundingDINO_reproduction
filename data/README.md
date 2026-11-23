# data/

Zbiory danych — **nie są w gicie** (`.gitignore`), notebooki pobierają je same.

```
data/
└── coco/                     # MS COCO 2017 (cocodataset.org)
    ├── val2017/              # 5000 obrazów walidacyjnych
    ├── annotations/          # instances_val2017.json (+ train, captions, keypoints)
    └── _downloads/           # oryginalne .zip — można usunąć po rozpakowaniu
```

Źródło (oficjalne, bez Kaggle):
- http://images.cocodataset.org/zips/val2017.zip
- http://images.cocodataset.org/annotations/annotations_trainval2017.zip

Nowe zbiory (Etap 3) dodawaj jako osobny katalog `data/<nazwa_zbioru>/`.
