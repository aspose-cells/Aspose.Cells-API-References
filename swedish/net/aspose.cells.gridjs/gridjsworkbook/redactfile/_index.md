---
title: "GridJsWorkbook.RedactFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridJsWorkbook metod. Utför radering på en Excel-fil baserat på en array av JSON-operationer"
type: docs
url: /sv/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

Utför redigering på en Excel-fil baserat på en array av JSON-operationer.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| excelFilePath | String | Filvägen till Excel-filen som ska raderas. |
| uid | String | Den unika identifieraren för arbetsboken. Om null eller tom, kommer ett nytt uid att genereras baserat på filvägen. |
| arrayOfRedactionOpr | String[] | En array av JSON-strängar som representerar de raderingsoperationer som ska tillämpas. |

### Undantag

| undantag | villkor |
| --- | --- |
| [GridCellException](../../gridcellexception/) | Kastas när ett CellsException inträffar under redigeringsoperationen. |
| Undantag | Kastas när ett allmänt undantag inträffar under redigeringsoperationen. |

### Se även

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


