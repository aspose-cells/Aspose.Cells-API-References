---
title: "SeriesCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection-metod. Lägger till Series-samlingen i ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Lägger till [`Series`](../../series/) samlingen i ett diagram.

```csharp
public int Add(string dataArea, bool isVertical)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dataArea | String | Anger värden som data-serien ska plottas från |
| isVertical | Boolean | Anger om serien ska plottas från ett intervall av cellvärden rad för rad eller kolumn för kolumn. Om true, [`Series`](../../series/) kommer att läggas till kolumn för kolumn. |

### Returvärde

Returnerar det första indexet för den tillagda ASeries i NSeries.

### Anmärkningar

Om data anges i sammanhängande celler, använd kolon för att separera dem. Till exempel $C$2:$C$5. Om data anges i icke‑sammanhängande celler, använd kommatecken för att separera dem. Till exempel: ($C$2,$D$5). Denna metod behandlar bara *dataArea* som dataintervall. Om du vill smart kontrollera metoden ChartCollection.Add().

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Skapa diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Lägg till serier med sträng- och booleska parametrar
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // Spara arbetsboken
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Lägger till [`Series`](../../series/) samlingen i ett diagram.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | String | Anger värden som data-serien ska plottas från |
| ärVertikal | Boolean | Anger om serien ska plottas från ett område med cellvärden radvis eller kolumnvis. |
| checkLabels | Boolean | Anger om intervallet innehåller seriens namn |

### Returvärde

Returnerar det första indexet för den tillagda ASeries i NSeries.

### Anmärkningar

Om data anges i sammanhängande celler, använd kolon för att separera dem. Till exempel $C$2:$C$5. Om data anges i icke‑sammanhängande celler, använd kommatecken för att separera dem. Till exempel ($C$2,$D$5).

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // Skapa diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Lägg till serier med Add‑metoden med sträng- och booleska parametrar
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // Spara arbetsboken
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


