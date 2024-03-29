---
title: Intersect
second_title: Aspose.Cells för .NET API-referens
description: Returnerar enRangeaspose.cells/range objekt som representerar den rektangulära skärningspunkten mellan två områden.
type: docs
weight: 320
url: /sv/net/aspose.cells/range/intersect/
---
## Range.Intersect method

Returnerar en[`Range`](../../range) objekt som representerar den rektangulära skärningspunkten mellan två områden.

```csharp
public Range Intersect(Range range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | Range | Det korsande området. |

### Returvärde

Returnerar a[`Range`](../../range) objekt

### Anmärkningar

Om de två områdena inte skärs, returneras null.

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();
// Få de första kalkylbladscellerna.
Cells cells = workbook.Worksheets[0].Cells;
Range range1 = cells.CreateRange("A1:A5");
Range range2 = cells.CreateRange("A3:A10");
//Hämta genomskärning av de två områdena.
Range intersectRange = range1.Intersect(range2);
//Spara Excel-filen
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()
'Skaffa de första kalkylbladscellerna.
Dim cells as Cells = workbook.Worksheets[0].Cells
Range range1 = cells.CreateRange("A1:A5")
Range range2 = cells.CreateRange("A3:A10")
'Få genomskärning av de två områdena.
Range intersectRange = range1.Intersect(range2)
'Spara Excel-filen
workbook.Save("book1.xlsm")
```

### Se även

* class [Range](../../range)
* namnutrymme [Aspose.Cells](../../range)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
