---
title: "LoadDataFilterOptions Enum"
linktitle: "LoadDataFilterOptions"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "LoadDataFilterOptions enum. Inkapslar objektet som representerar loaddatafilteroptions i Go."
type: docs
weight: 200
url: /sv/go-cpp/loaddatafilteroptions/
---

## LoadDataFilterOptions Enum

Representerar alternativen för att filtrera data när en arbetsbok laddas från en mall.

```go

type LoadDataFilterOptions int32


```

## Fält

| Fält | Beskrivning |
| --- | --- |
| [All](./all/) | Läs in alla |
| [CellBlank](./cellblank/) | Läs in celler vars värde är tomt |
| [CellString](./cellstring/) | Läs in celler vars värde är en sträng |
| [CellNumeric](./cellnumeric/) | Läs in celler vars värde är numeriskt (inklusive datumtid) |
| [CellError](./cellerror/) | Läs in celler vars värde är fel |
| [CellBool](./cellbool/) | Läs in celler vars värde är bool |
| [CellValue](./cellvalue/) | Läs in endast cellvärden (alla värdetyper) |
| [Formula](./formula/) | Läs in cellformler. |
| [CellData](./celldata/) | Läs in celldata inklusive värden, formler och formatering |
| [Chart](./chart/) | Läs in diagram |
| [Drawing](./drawing/) | Ritobjekt (inklusive diagram, bild, OleObject och alla andra ritobjekt) |
| [MergedArea](./mergedarea/) | Läs in sammanslagna celler |
| [ConditionalFormatting](./conditionalformatting/) | Läs in villkorsstyrd formatering |
| [DataValidation](./datavalidation/) | Läs in datavalideringar |
| [PivotTable](./pivottable/) | Läs in pivottabeller |
| [Table](./table/) | Läs in tabeller |
| [Hyperlinks](./hyperlinks/) | Läs in hyperlänkar |
| [SheetSettings](./sheetsettings/) | Läs in inställningar för arbetsblad |
| [SheetData](./sheetdata/) | Läs in all data för arbetsbladet, såsom celldata, inställningar, objekt, ...etc. |
| [BookSettings](./booksettings/) | Läs in inställningar för arbetsbok |
| [Settings](./settings/) | Läs in inställningar för arbetsbok och kalkylblad |
| [XmlMap](./xmlmap/) | Läs in XmlMap |
| [Structure](./structure/) | Läs in strukturen för arbetsboken |
| [Document_Properties](./document_properties/) | Läs in dokumentegenskaper |
| [DefinedNames](./definednames/) | Läs in definierade Name-objekt |
| [VBA](./vba/) | Läs in VBA-projekt |
| [Style](./style/) | Läs in stilar för cellformatering |
| [Picture](./picture/) | Läs in bilder |
| [OleObject](./oleobject/) | Läs in OleObjects |
| [Revision](./revision/) | Läs in revisionsloggar |
