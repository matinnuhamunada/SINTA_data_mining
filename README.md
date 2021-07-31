# SINTA_data_mining
Proyek iseng scraping peneliti _life sciences_ di Indonesia dari https://sinta.ristekbrin.go.id. 
Kunjungi tulisan saya mengenai output proyek ini di [**https://matinnuhamunada.github.io**](https://matinnuhamunada.github.io/posts/2021/07/sintalifesciences).

_Thanks to https://github.com/rendicahya/sinta-scraper for making this happen_

## _Goals_
Repository ini bertujuan untuk memetakan peneliti _life sciences_ di Indonesia. Dengan memetakan bidang keahlian peneliti _life sciences_, diharapkan kita dapat dengan mudah mencari kolaboran di berbagai institusi di Indonesia.

## Bagaimana kamu bisa berkontribusi?
Anda bisa berkontribusi dengan cara:
* Melakukan kurasi terhadap data, baik dengan mengisi tabel identitas peneliti secara manual, atau juga memberikan informasi mengenai peneliti yang sudah pensiun / tidak aktif.
* Memberikan rekomendasi peneliti atau institusi _life sciences_
* Mengolah dan menganalisis data
* Memberikan kritikan dan masukan :)

## _Repo structure_
```
├── README.md
├── data
│   └── {Universitas}
│       ├── data_NIDN-versi-sinta.txt #manually curated data
│       └── {Universitas}_bio_retired.txt #excluded authors
├── notebooks
│   ├── 00_data_scraping-{Universitas}.ipynb #scrape data and prepare for vis
│   └── 01_data_cleaning.ipynb #clean & initial visualization
├── scripts
│   └── author_search.py
├── envs
│   └── sinta.yml
├── tables
│   ├── {Universitas}_bio_clean.csv
│   └── {Universitas}_bio_ready.csv
└── figures
    └── bio_sinta.html # bokeh output
```

## _Ideas & To Dos_
* _Add search function in bokeh_
* _Bibliometric data scraping_
* _Author network analyses_
* _Wordcloud & Clustering_ topik penelitian
* [VOS viewer](https://www.vosviewer.com/)
* [Membuat semacam shiny App?](https://bibliometrix.org/)

_Thanks to this page on how to embed bokeh html_ [here](https://p-mckenzie.github.io/2017/12/01/embedding-bokeh-with-github-pages/)