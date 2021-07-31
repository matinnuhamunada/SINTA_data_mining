# SINTA_data_mining
Proyek iseng scraping peneliti _life sciences_ di Indonesia berdasarkan data di https://sinta.ristekbrin.go.id. Proyek ini berawal dari kesulitan saya menjawab pertanyaan seorang kolega: "Siapa sih pakar biologi molekuler di institusimu? Penelitiannya tentang apa?". 
Kunjungi juga tulisan saya mengenai output proyek ini di [https://matinnuhamunada.github.io](https://matinnuhamunada.github.io/posts/2021/07/sintalifesciences).

## Goals
Repository ini bertujuan untuk memetakan peneliti _life sciences_ di Indonesia. Dengan memetakan bidang keahlian peneliti _life sciences_, diharapkan kita dapat dengan mudah mencari kolaboran di berbagai institusi di Indonesia.

## _Warning & Caveats_
* _I am by no means someone experienced with bibliometric analyses_
* Informasi hanya didasarkan pada database SINTA sehingga afiliasi dan data peneliti belum tentu akurat
* Proyek ini tidak ditujukan untuk merangking atau membandingkan kualitas peneliti di suatu institusi. Indeks sitasi tidak sepenuhnya dapat digunakan untuk menilai kualitas seorang peneliti. Recommended reads di [https://theconversation.com](https://theconversation.com/jalan-evolusi-bibliometrik-indonesia-104781)
* Pemilihan institusi dan bidang ilmu peneliti sepenuhnya subjektif (bidang ilmu apa saja yang termasuk Life Sciences?)
 
## Bagaimana kamu bisa berkontribusi?
Anda bisa berkontribusi dengan cara:
* Melakukan kurasi terhadap data, baik dengan mengisi tabel identitas peneliti secara manual, atau juga memberikan informasi mengenai peneliti yang sudah pensiun / tidak aktif.
* Memberikan rekomendasi peneliti atau institusi _life sciences_
* Mengolah dan menganalisis data
* Memberikan kritikan dan masukan :)

## Data structure
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
    └── bio_sinta.html
```

## _Ideas & To Do's_
* Bibliometric data scraping
* _Author network analyses_
* [_Wordcloud & Clustering_ topik penelitian]
* [VOS viewer](https://www.vosviewer.com/)
* [Membuat semacam shiny App?](https://bibliometrix.org/)


