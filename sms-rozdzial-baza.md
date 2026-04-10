# Systematic Mapping Study

## Metoda badawcza

W pracy zastosowano **Systematic Mapping Study (SMS)** jako metodę wtórnej analizy literatury. SMS wybrano dlatego, że temat zastosowań AI i ML w środowiskach HPC jest szeroki, wielowątkowy i obejmuje wiele różnych klas problemów, takich jak planowanie zadań, predykcja wydajności, optymalizacja zużycia energii, detekcja awarii czy autotuning. W takim przypadku celem nie jest jeszcze precyzyjna synteza skuteczności jednej techniki, ale uporządkowanie pola badawczego i identyfikacja dominujących kierunków.

SMS pozwala odpowiedzieć na pytania o to, **jakie zastosowania są opisywane w literaturze, jakie metody AI/ML dominują, jakie typy ewaluacji są raportowane oraz gdzie widoczne są luki badawcze**. W odróżnieniu od klasycznego systematic literature review, podejście to koncentruje się przede wszystkim na mapowaniu obszaru, klasyfikacji prac i analizie trendów, a nie na szczegółowej syntezie efektów dla jednego wąskiego problemu.

## Zakres mapowania

Do badania włączane są publikacje, w których AI lub ML są stosowane **wewnątrz ekosystemu HPC**, to znaczy do wspierania zarządzania zasobami, przewidywania zachowania systemu, optymalizacji wykonania lub poprawy niezawodności środowiska obliczeniowego. Poza zakresem pozostają prace, w których HPC pełni wyłącznie rolę infrastruktury do trenowania modeli AI, bez bezpośredniego wkładu w problemy operacyjne lub systemowe HPC.

## Proces badawczy

Proces SMS obejmuje cztery główne etapy. Najpierw definiowany jest zakres badania, pytania badawcze oraz kryteria włączenia i wyłączenia publikacji. Następnie wykonywane jest systematyczne przeszukiwanie wybranych baz bibliograficznych przy użyciu zdefiniowanych ciągów wyszukiwawczych. W kolejnym kroku prowadzi się selekcję rekordów na podstawie tytułów, streszczeń i pełnych tekstów. Ostatni etap obejmuje ekstrakcję danych, budowę schematu klasyfikacji i przygotowanie mapy literatury.

## Schemat klasyfikacji

Na potrzeby pracy publikacje są klasyfikowane co najmniej według następujących osi:

- obszar zastosowania w HPC, np. scheduling, performance modeling, energy optimization, fault prediction,
- zastosowana technika AI/ML, np. klasyczne ML, deep learning, reinforcement learning,
- typ badania i typ ewaluacji,
- rodzaj środowiska HPC,
- raportowane metryki, np. czas wykonania, zużycie energii, wykorzystanie zasobów, dokładność predykcji.

Tak zdefiniowana mapa pozwala przedstawić nie tylko strukturę istniejącej literatury, ale też wskazać obszary dojrzałe, nisze badawcze i tematy wymagające dalszych badań.

## Rola narzędzi wspierających

W pracy można pomocniczo wykorzystać modele językowe do organizacji materiału, normalizacji słownictwa, sugerowania tagów klasyfikacyjnych i przygotowania roboczych podsumowań. Narzędzia te nie powinny jednak podejmować autonomicznych decyzji o włączeniu publikacji ani zastępować ręcznej ekstrakcji danych. Końcowe decyzje metodologiczne i interpretacyjne pozostają po stronie autora.

## Krótka wersja do bardzo zwartego artykułu

Jeśli w finalnym tekście zabraknie miejsca, rozdział można skrócić do poniższej wersji:

> W pracy zastosowano Systematic Mapping Study, ponieważ badany obszar - zastosowania AI i ML w HPC - ma szeroki i zróżnicowany charakter. Celem metody było uporządkowanie literatury, klasyfikacja publikacji według obszaru zastosowania, techniki AI/ML, typu ewaluacji i środowiska HPC oraz identyfikacja luk badawczych. Do analizy włączano wyłącznie prace, w których AI/ML wspierało problemy systemowe lub operacyjne HPC, a nie jedynie wykorzystywało infrastrukturę HPC do trenowania modeli. Proces obejmował zdefiniowanie pytań badawczych, systematyczne przeszukiwanie baz, selekcję publikacji oraz ekstrakcję i mapowanie danych.
