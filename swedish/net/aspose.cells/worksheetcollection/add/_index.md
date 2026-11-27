---
title: "WorksheetCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Lägger till ett kalkylblad i samlingen"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Lägger till ett kalkylblad i samlingen.

```csharp
public int Add(SheetType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | SheetType | Kalkylbladstyp. |

### Returvärde

[`Worksheet`](../../worksheet/) object index.

### Exempel

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
            
            // Lägg till ett nytt diagramblad med SheetType-parametern
            workbook.Worksheets.Add(SheetType.Chart);
            
            // Lägg till data i det första kalkylbladet
            Cells cells = workbook.Worksheets[0].Cells;
            cells["C2"].PutValue(5000);
            cells["C3"].PutValue(3000);
            cells["C4"].PutValue(4000);
            cells["C5"].PutValue(5000);
            cells["C6"].PutValue(6000);
            
            // Skapa diagram i diagrambladet
            Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
            int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
            Aspose.Cells.Charts.Chart chart = charts[chartIndex];
            chart.NSeries.Add("Sheet1!C2:C6", true);
            
            // Spara arbetsboken (valfritt)
            // workbook.Save(\"output.xlsx\");
        }
    }
}
```

### Se även

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

Lägger till ett kalkylblad i samlingen.

```csharp
public int Add()
```

### Returvärde

[`Worksheet`](../../worksheet/) object index.

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

Lägger till ett kalkylblad i samlingen.

```csharp
public Worksheet Add(string sheetName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | String | Arbetsbladsnamn |

### Returvärde

[`Worksheet`](../../worksheet/) object.

### Exempel

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
            
            // Lägg till data i det nya arbetsbladet
            worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
            
            // Spara arbetsboken
            wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


