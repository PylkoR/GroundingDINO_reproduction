# results/

Jeden katalog na eksperyment, w nim jeden podkatalog na uruchomienie (konfigurację):

```
results/
└── exp01_coco_zeroshot_val2017/          # eksperyment (notebook: src/notebooks/grounding_reproduction.ipynb)
    └── swint_ogc_hf__nall_seed42/        # run: <model>__n<liczba obrazów>_seed<seed>
        ├── config.json                   # model, prompt, rozmiar obrazu, liczba obrazów...
        ├── env.json                      # wersje bibliotek, GPU, czas inferencji
        ├── predictions.json              # surowe detekcje (format COCO results) — NIE w gicie
        ├── metrics_coco.json             # AP, AP50, AP75, APs/m/l, AR
        ├── comparison_with_paper.csv     # nasze vs artykuł
        ├── metrics_per_class.csv         # AP / AP50 per klasa
        ├── metrics_thresholded.json      # P, R, IoU, FP, FN przy box_threshold
        ├── metrics_thresholded_per_class.csv
        ├── threshold_sweep.csv           # P/R dla różnych box_threshold
        └── figures/                      # wykresy i przykłady (.png)
```

Kolejne eksperymenty: `exp02_<opis>/`, `exp03_<opis>/` ...
