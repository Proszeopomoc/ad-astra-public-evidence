
# AD ASTRA MCDO — PUBLICZNE PODSUMOWANIE STAGE3

## Cel

Pakiet przedstawia publiczny benchmark warstwy preselekcyjnej dla danych astronomicznych opartych o oznaczone dane KOI.

Warstwa publiczna celowo nie ujawnia:
- logiki scoringu,
- wag cech,
- mechanizmów routingu,
- szczegółów implementacyjnych.

Benchmark nie służy do potwierdzania planet.

Celem benchmarku jest:
- redukcja obciążenia,
- redukcja false positive,
- zachowanie wysokiego recall,
- uporządkowane trasowanie sygnałów.

---

# Wyniki

## Stage3A — KOI Benchmark

Profil recall 95%:

- recall średni: 0.9500
- precision średni: 0.6624
- redukcja false positive: 0.5118
- redukcja obciążenia: 0.2799

---

## Stage3B — Robustness Benchmark

Wyniki pozostały stabilne pomiędzy wieloma losowymi podziałami benchmarku.

Zaobserwowano:
- stabilność recall,
- stabilność workload reduction,
- stabilność routingu.

---

## Stage3C — Analiza szumu i anomalii

Odrzucone sygnały nie tworzą jednorodnego losowego szumu.

Zaobserwowano uporządkowane strumienie:
                        public_route  count  fraction
                   value-like stream   3830  0.416259
   signal-like false-positive stream   2303  0.250299
            anomaly-candidate stream   1445  0.157048
               typical reject stream    841  0.091403
       low-information reject stream    754  0.081948
value-labeled anomalous-shape stream     28  0.003043

To sugeruje, że:
- przestrzeń odrzuceń posiada strukturę,
- część anomalii może zawierać informację,
- routing zachowuje stabilną geometrię.

---

## Stage3D — Wizualizacja danych

Dołączone obrazy są projekcjami danych benchmarkowych.

Nie są:
- ilustracjami artystycznymi,
- mapami kosmosu,
- potwierdzeniem obiektów.

Ich celem jest pokazanie:
- separowalności,
- struktury routingu,
- geometrii benchmarku,
- podziału workloadu.

---

# Ograniczenia

Benchmark:
- nie potwierdza egzoplanet,
- nie zastępuje walidacji astrofizycznej,
- nie zastępuje pipeline NASA,
- nie stanowi dowodu odkrycia.

---

# Wniosek

Wyniki wskazują, że:
- preselekcja może ograniczać workload,
- wysoki recall może zostać zachowany,
- przestrzeń szumu nie jest losowa,
- routing pozostaje stabilny.

Pakiet ma charakter:
- evidence package,
- materiału partnerskiego,
- dokumentacji benchmarkowej.

Nie jest finalną publikacją naukową.
