---
title: "SeriesCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesCollection-Methode. Fügt die Series-Sammlung zu einem Diagramm hinzu"
type: docs
url: /de/net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Fügt die [`Series`](../../series/)-Sammlung zu einem Diagramm hinzu.

```csharp
public int Add(string dataArea, bool isVertical)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataArea | String | Gibt die Werte an, aus denen die Datenreihe geplottet wird |
| isVertical | Boolean | Gibt an, ob die Serie aus einem Zellwertbereich zeilenweise oder spaltenweise geplottet werden soll. Wenn true, wird [`Series`](../../series/) spaltenweise hinzugefügt. |

### Rückgabewert

Gibt den ersten Index der hinzugefügten ASeries in den NSeries zurück.

### Hinweise

Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie einen Doppelpunkt zur Trennung. Zum Beispiel $C$2:$C$5. Wenn Daten in nicht zusammenhängenden Zellen festgelegt werden, verwenden Sie ein Komma zur Trennung. Zum Beispiel: ($C$2,$D$5). Diese Methode verarbeitet lediglich *dataArea* als Datenbereich. Wenn Sie die Methode ChartCollection.Add() intelligent prüfen möchten.

### Beispiele

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
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Diagramm erstellen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Serie mit Zeichenketten- und Booleschen Parametern hinzufügen
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // Speichere die Arbeitsmappe
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Fügt die [`Series`](../../series/)-Sammlung zu einem Diagramm hinzu.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | String | Gibt die Werte an, aus denen die Datenreihe geplottet wird |
| isVertical | Boolean | Gibt an, ob die Reihe aus einem Zellbereich zeilenweise oder spaltenweise geplottet werden soll. |
| checkLabels | Boolean | Gibt an, ob der Bereich den Namen der Serie enthält |

### Rückgabewert

Gibt den ersten Index der hinzugefügten ASeries in den NSeries zurück.

### Hinweise

Wenn Daten in zusammenhängenden Zellen festgelegt werden, verwenden Sie einen Doppelpunkt zur Trennung. Zum Beispiel $C$2:$C$5. Wenn Daten in nicht zusammenhängenden Zellen festgelegt werden, verwenden Sie ein Komma zur Trennung. Zum Beispiel ($C$2,$D$5).

### Beispiele

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
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // Diagramm erstellen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Serie mit der Add-Methode und Zeichenketten- sowie Booleschen Parametern hinzufügen
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // Speichere die Arbeitsmappe
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


