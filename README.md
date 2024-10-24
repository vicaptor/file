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




## file 


| Aspekt                    | Media Layer                | Markup Language           |
|--------------------------|---------------------------|--------------------------|
| Główny focus             | Warstwy multimedialne     | Struktura dokumentu      |
| Najlepsze zastosowanie   | Opis scen i przestrzeni   | Semantyczny opis treści  |
| Podejście do struktury   | Warstwowe                 | Hierarchiczne            |
| Analogia                 | Jak warstwy w Photoshopie | Jak HTML/XML             |
| Rozszerzalność          | Przez dodawanie warstw    | Przez nowe znaczniki     |
| Kompatybilność          | Z systemami multimediów   | Z parsowaniem XML        |
| Złożoność przestrzenna  | Wyższa                    | Niższa                   |
| Złożoność semantyczna   | Niższa                    | Wyższa                   |



## law


| Cecha                    | SDML | NIEM | DFXML | CybOX | LIDO | UCO |
|-------------------------|------|------|-------|-------|------|-----|
| Opis fizycznej sceny    | ✓    | ✓    | ✗     | ✗     | ∼    | ∼   |
| Dowody cyfrowe          | ✓    | ✓    | ✓     | ✓     | ✗    | ✓   |
| Pozycjonowanie 3D       | ✓    | ✗    | ✗     | ✗     | ✗    | ✗   |
| Multimedia              | ✓    | ∼    | ∼     | ✗     | ✓    | ∼   |
| Łańcuch dowodowy        | ✓    | ✓    | ✓     | ∼     | ∼    | ✓   |
| Metadane prawne         | ✓    | ✓    | ✓     | ∼     | ∼    | ✓   |
| Prostota użycia         | ✓    | ✗    | ✓     | ∼    | ∼    | ∼   |


## standardy


| Standard | Element SDML | Element oryginalny |
|----------|-------------|-------------------|
| NIEM     | metadata    | CaseMetadata      |
| DFXML    | digital-evidence | fileobject   |
| CybOX    | digital-evidence | Observable   |
| LIDO     | evidence    | objectDescriptionSet |
| UCO      | chain-of-custody | ProvenanceRecord |




Porównanie SDML z UCO i NIEM:

1. UCO (Unified Cyber Ontology):

Różnice:
| Aspekt                  | SDML                          | UCO                           |
|------------------------|-------------------------------|-------------------------------|
| Format podstawowy      | XML, bardziej tradycyjny     | JSON-LD, nowoczesny RDF      |
| Zastosowanie          | Fizyczne + cyfrowe sceny     | Głównie cyfrowa forensyka    |
| Złożoność            | Średnia                      | Wysoka (pełna ontologia)     |
| Przestrzeń 3D         | Wbudowana                    | Ograniczona                   |
| Multimedia            | Natywne wsparcie            | Przez rozszerzenia           |
| Krzywa uczenia       | Łagodniejsza                 | Stroma (wymaga RDF/OWL)      |

2. NIEM (National Information Exchange Model):

Różnice:
| Aspekt                  | SDML                          | NIEM                          |
|------------------------|-------------------------------|-------------------------------|
| Zakres                | Skupiony na scenach           | Ogólny wymiana informacji    |
| Rozmiar              | Lżejszy                       | Bardzo rozbudowany           |
| Elastyczność         | Wyższa                        | Niższa (ścisłe reguły)       |
| Implementacja        | Prostsza                      | Złożona                      |
| Zgodność            | Mniej restrykcyjna            | Bardzo restrykcyjna          |
| Specjalizacja       | Sceny i multimedia            | Wszystkie aspekty prawne     |

3. Korzyści SDML:

a) Techniczne:
```xml
<!-- SDML - Prosty opis pozycji 3D -->
<position>
    <coordinates x="2.5" y="1.8" z="0"/>
    <orientation>45</orientation>
</position>

<!-- NIEM - Bardziej złożony odpowiednik -->
<niem:LocationTwoDimensionalGeographicCoordinate>
    <niem:GeographicCoordinateLatitude>
        <niem:LatitudeDegreeValue>52.2297</niem:LatitudeDegreeValue>
    </niem:GeographicCoordinateLatitude>
    <!-- ... wiele więcej znaczników ... -->
</niem:LocationTwoDimensionalGeographicCoordinate>

<!-- UCO - Wymaga ontologii -->
{
  "@type": "location:Location",
  "location:latitude": "52.2297",
  "location:longitude": "21.0122",
  "uco-core:hasFacet": {
    "@type": "location:LatLongCoordinatesFacet"
    // ... złożona struktura RDF ...
  }
}
```

b) Praktyczne korzyści SDML:

1. Prostsze wdrożenie:
```python
# SDML - Prosty parser
def parse_sdml_position(xml_node):
    return {
        'x': float(xml_node.find('coordinates').get('x')),
        'y': float(xml_node.find('coordinates').get('y')),
        'z': float(xml_node.find('coordinates').get('z'))
    }

# NIEM/UCO - Bardziej złożona implementacja
def parse_niem_position(niem_node):
    # Wymaga znacznie więcej kodu i obsługi złożonych struktur
    pass
```

2. Efektywniejsze przechowywanie:
```xml
<!-- SDML - Kompaktowy zapis -->
<evidence id="E001">
    <position x="2.5" y="1.8" z="0"/>
    <description>Nóż kuchenny</description>
</evidence>

<!-- NIEM - Więcej narzutu -->
<niem:EvidenceItem>
    <niem:EvidenceItemID>
        <nc:IdentificationID>E001</nc:IdentificationID>
    </niem:EvidenceItemID>
    <niem:EvidenceDescription>
        <nc:DescriptionText>Nóż kuchenny</nc:DescriptionText>
    </niem:EvidenceDescription>
    <!-- ... więcej metadanych ... -->
</niem:EvidenceItem>
```

3. Główne zalety SDML:

a) W porównaniu z UCO:
- Prostszy w implementacji
- Lepsze wsparcie dla fizycznych scen
- Łatwiejszy w nauce i użyciu
- Mniejsze wymagania techniczne
- Lepsze wsparcie dla multimediów

b) W porównaniu z NIEM:
- Bardziej skupiony na konkretnym zastosowaniu
- Mniejsza złożoność
- Szybsze wdrożenie
- Lepsza obsługa przestrzeni 3D
- Elastyczniejsza struktura

4. Sytuacje gdzie SDML jest lepszy:

a) Dokumentacja miejsca zdarzenia:
- Dokładniejsze opisy przestrzenne
- Łatwiejsza integracja z narzędziami 3D
- Lepsze wsparcie dla fotografii i wideo

b) Małe i średnie organizacje:
- Niższe koszty wdrożenia
- Mniejsze wymagania szkoleniowe
- Szybsze rozpoczęcie pracy

c) Projekty multimedialne:
- Lepsza integracja z systemami wizualizacji
- Wsparcie dla streamingu
- Efektywniejsza obsługa metadanych


