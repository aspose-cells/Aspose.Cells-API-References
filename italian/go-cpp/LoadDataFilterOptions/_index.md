---
title: "LoadDataFilterOptions Enum"
linktitle: "LoadDataFilterOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Enum LoadDataFilterOptions. Incapsula l'oggetto che rappresenta loaddatafilteroptions in Go."
type: docs
weight: 200
url: /it/go-cpp/loaddatafilteroptions/
---

## LoadDataFilterOptions Enum

Rappresenta le opzioni per filtrare i dati durante il caricamento della cartella di lavoro da un modello.

```go

type LoadDataFilterOptions int32


```

## Campi

| Campo | Descrizione |
| --- | --- |
| [All](./all/) | Carica tutto |
| [CellBlank](./cellblank/) | Carica le celle il cui valore è vuoto |
| [CellString](./cellstring/) | Carica le celle il cui valore è una stringa |
| [CellNumeric](./cellnumeric/) | Carica le celle il cui valore è numerico (inclusi data/ora) |
| [CellError](./cellerror/) | Carica le celle il cui valore è errore |
| [CellBool](./cellbool/) | Carica le celle il cui valore è booleano |
| [CellValue](./cellvalue/) | Carica solo il valore delle celle (tutti i tipi di valore) |
| [Formula](./formula/) | Carica le formule delle celle. |
| [CellData](./celldata/) | Carica i dati delle celle includendo valori, formule e formattazione |
| [Chart](./chart/) | Carica i grafici |
| [Drawing](./drawing/) | Oggetti di disegno (inclusi Chart, Picture, OleObject e tutti gli altri oggetti di disegno) |
| [MergedArea](./mergedarea/) | Carica le celle unite |
| [ConditionalFormatting](./conditionalformatting/) | Carica la formattazione condizionale |
| [DataValidation](./datavalidation/) | Carica le convalide dei dati |
| [PivotTable](./pivottable/) | Carica le tabelle pivot |
| [Table](./table/) | Carica le tabelle |
| [Hyperlinks](./hyperlinks/) | Carica i collegamenti ipertestuali |
| [SheetSettings](./sheetsettings/) | Carica le impostazioni del foglio di lavoro |
| [SheetData](./sheetdata/) | Carica tutti i dati del foglio di lavoro, come dati delle celle, impostazioni, oggetti, ...ecc. |
| [BookSettings](./booksettings/) | Carica le impostazioni per la cartella di lavoro |
| [Settings](./settings/) | Carica le impostazioni per la cartella di lavoro e il foglio di lavoro |
| [XmlMap](./xmlmap/) | Carica XmlMap |
| [Structure](./structure/) | Carica la struttura della cartella di lavoro |
| [Document_Properties](./document_properties/) | Carica le proprietà del documento |
| [DefinedNames](./definednames/) | Carica gli oggetti Name definiti |
| [VBA](./vba/) | Carica i progetti VBA |
| [Style](./style/) | Carica gli stili per la formattazione delle celle |
| [Picture](./picture/) | Carica le immagini |
| [OleObject](./oleobject/) | Carica OleObjects |
| [Revision](./revision/) | Carica i registri di revisione |
