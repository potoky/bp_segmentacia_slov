# Segmentácia Slovenských slov program



## Intro

Programová časť bakalárskej práce Segmentácia Slovenských slov na morfémy pomocou strojového učenia.

## Klonovanie súborov

Pomocou týchto príkazov zadaných do terminálu si naklonujete programový repozitár do svojho pracovného prostredia:

```
root # cd any_local_dir
any_local_dir # git clone https://git.kpi.fei.tuke.sk/kpi-zp/2024/bp.anna.potocka/segmentacia-slovenskych-slov-program.git
```

## Prehľad repozitára

Obsah adresára, ktorý ste si práve naklonovali do svojho počítača je hierarchicky usporiadaný takto:
```
.
├── README.md
└── src
    ├── fasttext
    │   ├── data_scaler.py
    │   ├── fasttext.py
    │   ├── ft_vector_dataset.py
    │   ├── main.py
    │   ├── ohe_segments.py
    │   ├── one_words.py
    │   └── ft_files
    │       ├── ft_model
    │       ├── rmss_ft_vector_data_path.csv
    │       ├── rmss_ohe_segments_data.csv
    │       ├── rmss_words_data.txt
    │       └── scaler.save
    ├── additional_src
    │   ├── data_prep.py
    │   ├── load_data_from_excel.py
    │   ├── main_cnn.ipynb
    │   ├── main_cnn.py
    │   ├── main_dense.ipynb
    │   ├── main_dense.py
    │   ├── simplify_data.py
    │   ├── variables.py
    │   └── word_classed_data.py
    ├── files
    │   ├── RMSS-na-analyzu.xlsx
    │   ├── rmss_simple_data.csv
    │   └── vysledky.xlsx
    ├── dense.py
    └── main.py
```

Pre vypísanie hierarchie vo vlastnom počítači použite nasledujúce príkazy:

```
root # sudo apt-get install tree
root # tree /any_local_dir
any_local_dir # tree
```

## Nastavenie VS Code na spracovanie vstupu pre Python skript

- [ ] [Nainštalovanie rozšírenia Code Runner](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- [ ] VS Code -> Preferences -> Settings
- [ ] Vyhľadajte a zaznačte položku Code-runner: Run In Terminal

## Otvorenie a spustenie programu

Nie je nutné otvorenie programu v editore. Program sa dá spustiť v terminály za predpokladu, že máte nainštalované všetky potrebné knižnice.
Navigujte sa do adresára, v ktorom sa nachádza súbor main.py a dense.py alebo zadajte pri spúšťaní celý názov cesty súboru main.py.
Ak ste v prostredí VS Code, zobrazte tento súbor pomocou klinutia naň v okne Explorer.

```
.
├── README.md
└── src
    ├── dense.py
    └── main.py
```

V termináli zadajte tento príkaz:

```
src # python main.py
```

alebo:

```
any_local_dir # python segmentacia-slovenskych-slov-program/src/main.py
```

V editore VS Code je možné spustiť program pomocou ikony ▶️ v pravom hornom rohu otvoreného okna skriptu.
