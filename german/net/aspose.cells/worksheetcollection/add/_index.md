---
title: "WorksheetCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Fügt ein Arbeitsblatt zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Fügt der Sammlung ein Arbeitsblatt hinzu.

```csharp
public int Add(SheetType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | SheetType | Arbeitsblatttyp. |

### Rückgabewert

[`Worksheet`](../../worksheet/) object index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithSheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Füge ein neues Diagrammblatt mit dem SheetType-Parameter hinzu
            workbook.Worksheets.Add(SheetType.Chart);
            
            // Füge Daten zum ersten Arbeitsblatt hinzu
            Cells cells = workbook.Worksheets[0].Cells;
            cells["C2"].PutValue(5000);
            cells["C3"].PutValue(3000);
            cells["C4"].PutValue(4000);
            cells["C5"].PutValue(5000);
            cells["C6"].PutValue(6000);
            
            // Erstelle ein Diagramm im Diagrammblatt
            Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
            int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
            Aspose.Cells.Charts.Chart chart = charts[chartIndex];
            chart.NSeries.Add("Sheet1!C2:C6", true);
            
            // Arbeitsmappe speichern (optional)
            // workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

Fügt der Sammlung ein Arbeitsblatt hinzu.

```csharp
public int Add()
```

### Rückgabewert

[`Worksheet`](../../worksheet/) object index.

### Siehe auch

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

Fügt der Sammlung ein Arbeitsblatt hinzu.

```csharp
public Worksheet Add(string sheetName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetName | String | Arbeitsblattname |

### Rückgabewert

[`Worksheet`](../../worksheet/) object.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets.Add("NewSheet");
            
            // Füge Daten zum neuen Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
            
            // Speichere die Arbeitsmappe
            wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


