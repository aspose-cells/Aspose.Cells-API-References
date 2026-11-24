---
title: "ChartCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartCollection‑Methode. Fügt ein Diagramm zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells.charts/chartcollection/add/
---
## Add(ChartType, int, int, int, int) {#add}

Fügt ein Diagramm zur Sammlung hinzu.

```csharp
public int Add(ChartType type, int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ChartType | Diagrammtyp |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| bottomRow | Int32 | Index der unteren rechten Zeile |
| rightColumn | Int32 | Index der unteren rechten Spalte |

### Rückgabewert

[`Chart`](../../chart/) object index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 1; i <= 10; i++)
            {
                sheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
                sheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Ein Diagramm mit den angegebenen Parametern hinzufügen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("=Sheet1!$A$1:$B$11", true);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, int, int, int, int) {#add_2}

Fügt ein Diagramm zur Sammlung hinzu.

```csharp
[Obsolete("Use ChartCollection.Add(ChartType, string, bool ,int , int, int, int ) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ChartType type, string dataRange, int topRow, int leftColumn, int rightRow, 
    int bottomColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ChartType | Diagrammtyp |
| dataRange | String | Gibt den Datenbereich des Diagramms an |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| rightRow | Int32 | Index der unteren rechten Zeile |
| bottomColumn | Int32 | Index der unteren rechten Spalte |

### Rückgabewert

[`Chart`](../../chart/) object index.

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die `Add`‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Mai 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithChartTypeStringInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            try
            {
                // Rufen Sie die Add‑Methode mit den Parametern (ChartType, String, Int32, Int32, Int32, Int32) auf
                int chartIndex = worksheet.Charts.Add(
                    ChartType.Column,          // Chart type
                    "A1:B4",                  // Data range
                    0,                        // Top row position
                    3,                        // Left column position
                    15,                       // Bottom row position
                    8                         // Right column position
                );

                Console.WriteLine("Chart added successfully at index: " + chartIndex);
                
                // Greifen Sie auf das neu erstellte Diagramm zu
                Chart chart = worksheet.Charts[chartIndex];
                chart.Title.Text = "Sample Column Chart";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("ChartCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(byte[], string, bool, int, int, int, int) {#add_3}

Fügt ein Diagramm mit vordefinierter Vorlage hinzu.

```csharp
public int Add(byte[] data, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Daten | Byte[] | Die Daten der Diagrammvorlagendatei (.crtx). |
| dataRange | String | Gibt den Datenbereich des Diagramms an |
| isVertical | Boolean | Gibt an, ob die Reihe aus einem Zellbereich zeilenweise oder spaltenweise geplottet werden soll. |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| rightRow | Int32 | Index der unteren rechten Zeile |
| bottomColumn | Int32 | Index der unteren rechten Spalte |

### Rückgabewert

[`Chart`](../../chart/) object index.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionMethodAddWithByteArrayStringBooleanInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Erstellen Sie ein Byte‑Array, das Diagrammdaten darstellt (vereinfachtes Beispiel)
            byte[] chartData = new byte[] { 0x01, 0x02, 0x03 };

            try
            {
                // Rufe die Add-Methode mit spezifischen Parametern auf
                int chartIndex = worksheet.Charts.Add(
                    chartData,          // Byte[] data
                    "A1:B4",            // String dataRange
                    true,               // Boolean isVertical
                    0,                  // Int32 topRow
                    0,                  // Int32 leftColumn
                    15,                 // Int32 rightRow
                    8                   // Int32 bottomColumn
                );

                Console.WriteLine($"Chart added successfully at index: {chartIndex}");

                // Greifen Sie auf das hinzugefügte Diagramm zu
                Chart chart = worksheet.Charts[chartIndex];
                chart.Type = ChartType.Column;

                // Ergebnis speichern
                workbook.Save("ChartCollectionMethodAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(ChartType, string, bool, int, int, int, int) {#add_1}

Fügt ein Diagramm zur Sammlung hinzu.

```csharp
public int Add(ChartType type, string dataRange, bool isVertical, int topRow, int leftColumn, 
    int rightRow, int bottomColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ChartType | Diagrammtyp |
| dataRange | String | Gibt den Datenbereich des Diagramms an |
| isVertical | Boolean | Gibt an, ob die Reihe aus einem Zellbereich zeilenweise oder spaltenweise geplottet werden soll. |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| rightRow | Int32 | Index der unteren rechten Zeile |
| bottomColumn | Int32 | Index der unteren rechten Spalte |

### Rückgabewert

[`Chart`](../../chart/) object index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddWithChartTypeStringBooleanInt32IntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["C3"].PutValue(40);

            // Diagramm mit angegebenen Parametern hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, "A1:C3", true, 4, 4, 14, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


