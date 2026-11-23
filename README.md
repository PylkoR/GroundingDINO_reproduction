# Grounding DINO — reprodukcja (ADOM, temat 10)

Artykuł: Liu et al., *Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection*, arXiv:2303.05499.

## Środowisko
```bash
uv sync                      # tworzy .venv z pyproject.toml / uv.lock
```
W VS Code jako kernel notebooka wybierz `.venv/bin/python`.

## Struktura
```
data/            zbiory danych (pobierane automatycznie, poza gitem) — patrz data/README.md
results/         wyniki eksperymentów: exp<NN>_<opis>/<run>/ — patrz results/README.md
src/notebooks/   notebooki
presentations/   prezentacje, karta projektu, artykuł
```

## Eksperymenty
| ID | Notebook | Opis |
|---|---|---|
| exp01 | `src/notebooks/grounding_reproduction.ipynb` | Grounding DINO-T zero-shot na COCO val2017, porównanie z Tab. 2 (AP 48.4) |
