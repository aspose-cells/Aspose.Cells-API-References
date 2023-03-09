---
title: metodo create_safe_sheet_name
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 90
url: /it/python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---
##  create_safe_sheet_name(name_proposal) {#str}
Controlla il nome del foglio specificato e ne crea uno valido quando necessario.
Se il nome del foglio specificato è conforme alle regole del nome del foglio Excel, restituiscilo.
Altrimenti la stringa verrà troncata se la lunghezza supera il limite
e i caratteri non validi verranno sostituiti con ' ', quindi restituiranno il valore della stringa ricostruita.


###  ritorna




```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| name_proposal | str | nome del foglio da utilizzare|


##  create_safe_sheet_name(name_proposal, replace_char) {#str-char}
Controlla il nome del foglio specificato e ne crea uno valido quando necessario.
Se il nome del foglio specificato è conforme alle regole del nome del foglio Excel, restituiscilo.
Altrimenti la stringa verrà troncata se la lunghezza supera il limite
i caratteri non validi verranno sostituiti con il carattere specificato, quindi restituiranno il valore della stringa ricostruita.


###  ritorna




```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| name_proposal | str | nome del foglio da utilizzare|
| replace_char | char | carattere che verrà utilizzato per sostituire i caratteri non validi nel nome del foglio specificato|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [CellsHelper](/cells/it/python-net/aspose.cells/cellshelper)
