# file format

Pełna nazwa standardu: "SMDF - Stream Media Description File Format"

## .smdf - Stream Media Description File

S - Stream (strumień)
M - Media (multimedia)
D - Description (opis)
F - File (plik)

Zalety tej wersji:

Description vs Described:

Description sugeruje zawartość/komponent
Lepiej oddaje, że plik ZAWIERA opisy
Bardziej techniczne określenie
Jaśniej wskazuje na format zawierający metadane opisowe


Struktura nazwy:

Stream - typ przekazu
Media - rodzaj zawartości
Description - kluczowa funkcja/cecha
File - format


Zastosowania:

live.smdf
vod.smdf
stream.smdf
broadcast.smdf



## konflikty dla SMDF (Stream Media Description File):

Znane konflikty .smdf:
1. Structured Material Data File (.smdf) - w inżynierii materiałowej, ale rzadko używany
2. Shared Memory Data File (.smdf) - w niektórych systemach, ale nie jest powszechny
3. Smart Media Device Format (.smdf) - starsza technologia, już mało używana

## Analiza konfliktu:

1. Poziom konfliktu:
- Niski do średniego
- Istniejące użycia są niszowe
- Niektóre formaty są przestarzałe
- Brak powszechnie używanego standardu z tym rozszerzeniem

2. Kontekst użycia:
- Inne dziedziny (materiałoznawstwo, systemy operacyjne)
- Inne zastosowania
- Małe ryzyko pomyłki ze względu na różne konteksty

3. Zalety utrzymania .smdf:
- Intuicyjne rozszerzenie
- Dobrze opisuje zawartość
- Istniejące konflikty nie są krytyczne
- Można użyć w specyficznym kontekście streamingu

### Wniosek: 

Konflikty istnieją, ale są na tyle małe i w innych dziedzinach, że .smdf wydaje się nadal dobrym wyborem dla Stream Media Description File.



| Cecha                  | SDML | IMSC | EBU-TT | DFXP | SMIL | TTML |
|-----------------------|------|------|--------|------|------|------|
| Napisy                | ✓    | ✓    | ✓      | ✓    | ✓    | ✓    |
| Audiodeskrypcja       | ✓    | ×    | ×      | ×    | ∼    | ×    |
| Metadane mediów       | ✓    | ∼    | ✓      | ∼    | ∼    | ∼    |
| Synchronizacja        | ✓    | ✓    | ✓      | ✓    | ✓    | ✓    |
| Stylowanie            | ✓    | ✓    | ✓      | ✓    | ∼    | ✓    |
| Pozycjonowanie        | ✓    | ✓    | ✓      | ✓    | ✓    | ✓    |
| Wielojęzyczność      | ✓    | ✓    | ✓      | ✓    | ✓    | ✓    |
| Streaming            | ✓    | ∼    | ∼      | ×    | ∼    | ×    |
| Opis scen            | ✓    | ×    | ×      | ×    | ∼    | ×    |
| Walidacja XSD        | ✓    | ✓    | ✓      | ✓    | ✓    | ✓    |


