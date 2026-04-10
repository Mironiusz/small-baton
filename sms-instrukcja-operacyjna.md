## 2. Definicja zakresu

### Wchodzi do badania

Publikacja wchodzi, jeśli AI lub ML są użyte do rozwiązania problemu **wewnątrz HPC**, np.:

- scheduling,
- resource allocation,
- workload prediction,
- performance prediction / modeling,
- anomaly detection,
- fault prediction,
- resilience,
- energy optimization,
- autotuning,
- runtime optimization,
- code optimization dla HPC.

### Nie wchodzi do badania

Publikacja nie wchodzi, jeśli:

- HPC służy tylko do trenowania modelu AI,
- temat dotyczy ogólnie AI for science bez problemu systemowego HPC,
- nie ma realnej metody AI/ML,
- to tylko opis narzędzia, keynote, editorial lub krótki poster bez metody.

---

## 3. Minimalny zestaw rzeczy do przygotowania

Przed startem musisz mieć:

- temat i zakres badania zapisane w 3-5 zdaniach,
- listę research questions,
- listę baz,
- wstępne search stringi,
- kryteria inclusion / exclusion,
- arkusz do screeningu,
- arkusz do ekstrakcji danych,
- folder na PDF-y,
- log decyzji.

### Narzędzia

Praktyczny zestaw:

- Zotero lub Mendeley do bibliografii,
- Rayyan albo Excel / Google Sheets do screeningu,
- Excel / Sheets / Airtable do ekstrakcji,
- Python / R / Excel do wykresów,
- LLM do pomocy przy tagowaniu i roboczych notatkach.

---

## 4. Research questions - wzór

Możesz przyjąć taki zestaw:

**RQ1.** Jakie obszary zastosowań AI/ML w HPC są opisywane w literaturze?

**RQ2.** Jakie algorytmy sztucznej inteligencji są stosowane w tych obszarach?

**RQ3.** Jakie algorytmy są obecnie uznawane za najskuteczniejsze?

**RQ4.** Jakie środowiska HPC i jakie metryki są używane do oceny?

---

## 5. Bazy danych

### Rdzeń

- Scopus
- Web of Science Core Collection
- IEEE Xplore
- ACM Digital Library

### Opcjonalnie

- Compendex
- Inspec
- SpringerLink jako uzupełnienie
- arXiv tylko wtedy, gdy jawnie dopuszczasz preprinty

---

## 6. Budowa search stringów

### Krok 1. Zbuduj trzy bloki pojęć

#### Blok A - AI/ML

```text
"artificial intelligence" OR "machine learning" OR "deep learning" OR "neural network*" OR "reinforcement learning" OR "graph neural network*" OR "predictive model*"
```

#### Blok B - HPC

```text
"high performance computing" OR HPC OR supercomput* OR "parallel computing" OR "cluster computing" OR exascale OR petascale OR "heterogeneous computing"
```

#### Blok C - problemy HPC

```text
schedul* OR "resource allocation" OR "workload prediction" OR "performance prediction" OR "performance modeling" OR "anomaly detection" OR "fault prediction" OR resilience OR "energy optimization" OR autotun* OR "runtime optimization" OR "job placement" OR "load balancing"
```

### Krok 2. Zbuduj dwa query

#### Query szerokie

```text
("artificial intelligence" OR "machine learning" OR "deep learning" OR "neural network*" OR "reinforcement learning" OR "graph neural network*" OR "predictive model*")
AND
("high performance computing" OR HPC OR supercomput* OR "parallel computing" OR "cluster computing" OR exascale OR petascale OR "heterogeneous computing")
```

#### Query zawężone

```text
("artificial intelligence" OR "machine learning" OR "deep learning" OR "neural network*" OR "reinforcement learning" OR "graph neural network*" OR "predictive model*")
AND
("high performance computing" OR HPC OR supercomput* OR "parallel computing" OR "cluster computing" OR exascale OR petascale OR "heterogeneous computing")
AND
(schedul* OR "resource allocation" OR "workload prediction" OR "performance prediction" OR "performance modeling" OR "anomaly detection" OR "fault prediction" OR resilience OR "energy optimization" OR autotun* OR "runtime optimization" OR "job placement" OR "load balancing")
```

### Krok 3. Dopasuj składnię do bazy

#### Scopus

```text
TITLE-ABS-KEY(...)
```

#### Web of Science

```text
TS=(...)
```

#### IEEE Xplore

Szukaj w metadata, abstract i index terms.

#### ACM DL

Szukaj w title, abstract, keywords.

---

## 7. Walidacja query

Przed pełnym search-em zbierz ręcznie 15-30 paperów, które na pewno są trafne.

### Cel

Sprawdzić, czy query łapie większość sensownych prac.

### Reguła

Jeżeli query nie łapie dużej części znanych trafnych publikacji, poprawiasz:

- synonimy,
- zakres pojęć HPC,
- zakres pojęć problemowych,
- operatory logiczne.

Nie odpalaj dużego searchu, dopóki query nie jest sensowne.

---

## 8. Algorytm przeszukiwania - krok po kroku

### Etap A - search bazodanowy

1. Uruchom query w każdej bazie.
2. Eksportuj rekordy z metadanymi.
3. Zapisz liczbę wyników per baza.
4. Połącz rekordy w jeden zbiór.
5. Zrób deduplikację.

### Pola do eksportu

Eksportuj, jeśli baza pozwala:

- title,
- authors,
- year,
- abstract,
- keywords,
- source / venue,
- DOI,
- link,
- citation count.

### Deduplikacja

Rób w tej kolejności:

1. DOI,
2. title po normalizacji,
3. title + first author + year.

---

## 9. Screening - algorytm decyzyjny

### Poziom 1 - title + abstract

Dla każdego rekordu nadaj jedną z decyzji:

- Include
- Exclude
- Uncertain = Exclude

### Decision rules

#### Include

Daj Include, jeśli z tytułu i abstraktu wynika, że:

- temat dotyczy HPC,
- użyto AI/ML,
- AI/ML rozwiązuje problem operacyjny, systemowy lub optymalizacyjny HPC.

#### Exclude

Daj Exclude, jeśli:

- HPC to tylko platforma uruchomieniowa,
- nie ma AI/ML,
- nie da się uznać pracy za publikację naukową z metodą,
- temat ewidentnie nie pasuje do scope,
- artykuł starszy niż 2020.

---

## 10. Snowballing - algorytm przeszukiwania artykułów

Po zbudowaniu wstępnego korpusu z baz robisz dwa dodatkowe search-e.

### Backward snowballing

Dla każdego włączonego papera, głębokość = 1:

1. przeglądasz bibliografię,
2. zaznaczasz potencjalnie trafne pozycje,
3. sprawdzasz ich metadane,
4. przeprowadzasz ten sam screening.

### Forward snowballing

Dla każdego kluczowego papera, głębokość = 1:

1. sprawdzasz, kto go cytuje,
2. wybierasz potencjalnie trafne pozycje,
3. przeprowadzasz screening.

### Warunek stopu

Kończysz, gdy kolejna iteracja nie wnosi prawie żadnych nowych, trafnych publikacji.

---

## 11. Manual search (Ewentualnie)

Na końcu przejrzyj ręcznie ważne venue, np.:

- SC,
- IPDPS,
- Cluster,
- JPDC,
- FGCS,
- IEEE TPDS,
- Concurrency and Computation.

To jest ważne zwłaszcza wtedy, gdy nazewnictwo w paperach jest niestabilne.

---

## 12. Schemat klasyfikacji

Dla każdego włączonego paperu przypisz co najmniej poniższe pola.

### Oś 1 - obszar zastosowania, ona separuje tabele (do edycji)

- scheduling
- resource allocation
- workload prediction
- performance modeling
- anomaly detection
- fault prediction
- resilience
- energy optimization
- autotuning
- runtime optimization
- code optimization
- storage / I/O optimization

### Oś 2 - technika AI/ML (do edycji)

- classical ML
- deep learning
- reinforcement learning
- graph-based models
- probabilistic methods
- ensemble methods
- LLM / foundation model
- hybrid methods

### Oś 3 - typ badania

- solution proposal
- validation research
- evaluation research
- experience report
- review / secondary study

### Oś 4 - typ ewaluacji (do edycji)

- simulation
- trace-driven evaluation
- benchmark
- real cluster deployment
- production data
- synthetic data

### Oś 5 - środowisko HPC (do edycji)

- CPU cluster
- GPU cluster
- heterogeneous cluster
- cloud-HPC
- exascale / pre-exascale
- unspecified

### Oś 6 - metryki (do edycji)

- makespan
- throughput
- queue waiting time
- utilization
- energy
- accuracy
- overhead
- scalability

---

## 13. Formularz ekstrakcji danych - wzór

Skopiuj to do arkusza jako kolumny:

```text
ID
Source type (typ źródła publikacji np. konferencja, review)
Database origin (z której bazy)
DOI
Title
Authors
Year 
Venue (miejsce publikacji typu nazwa czasopisma / nazwa konferencji)
Country / affiliation 
Problem area in HPC (po tym grupujemy artykuły)
AI/ML technique
Input data type (tylko dla wybranych artykułów; dane na wejściu algorytmu / modelu)
Output / decision type (tylko dla wybranych artykułów; dane na wyjściu algorytmu / modelu)
Research type (typ badań)
Evaluation type (sposób oceny jakości rozwiązania)
HPC environment (dokładniejsze środowisko)
Metrics (metryki użyte do jakości rozwiązania)
Main contribution (podsumowanie abstraktu)
Main result (podsumowanie efektów pracy)
Limitations (ograniczenia)
Include decision (either: no / include by team member)
Notes (komentarze)
```

---

## 14. Jak używać LLM w tym procesie

Można używać LLMów do dwóch rzeczy:
1. streszczenie artykułu pod uprzednio spromptowaną full-text analizę
2. wstępne uzupełnienie formularza ekstrakcji danych dla artykułu. Wymaga każdorazowego sprawdzenia przez człowieka.

Używany model oraz dokładny prompt będą pokazane w artykule.