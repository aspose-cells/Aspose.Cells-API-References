---
title: "Name.GetRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Methode. Gibt den Bereich zurück, wenn dieser Name auf einen Bereich verweist"
type: docs
url: /de/net/aspose.cells/name/getrange/
---
## GetRange() {#getrange}

Liest den Bereich, wenn sich dieser Name auf einen Bereich bezieht.

```csharp
public Range GetRange()
```

### Rückgabewert

Der Bereich.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            
            // Benannten Bereich erstellen
            int index = workbook.Worksheets.Names.Add("MyRange");
            workbook.Worksheets.Names[index].RefersTo = "=Sheet1!A1:B3";
            Name namedRange = workbook.Worksheets.Names[index];
            
            // GetRange-Methode demonstrieren
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Named Range Address: " + range.Address);
            Console.WriteLine("Worksheet Name: " + range.Worksheet.Name);
            
            // Den Bereich ändern
            foreach (Cell cell in range)
            {
                if (cell.Row == 0)
                {
                    cell.PutValue(cell.StringValue.ToUpper());
                }
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(bool) {#getrange_1}

Liest den Bereich, wenn sich dieser Name auf einen Bereich bezieht

```csharp
public Range GetRange(bool recalculate)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| neu berechnen | Boolean | ob es neu berechnet wird, wenn dieser Name bereits vor diesem Aufruf berechnet wurde. |

### Rückgabewert

Der Bereich.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten befüllen
            for (int i = 0; i < 4; i++)
            {
                cells[i, 1].PutValue(i); // Column B values: 0,1,2,3
            }

            // Einen benannten Bereich mit Formel erstellen
            int nameIndex = wb.Worksheets.Names.Add("testname");
            Name name = wb.Worksheets.Names[nameIndex];
            name.RefersTo = "IFERROR(Sheet1!$B$2:$B$4,-1)";

            // Verwenden Sie den benannten Bereich in Formeln
            cells["C1"].Formula = "=testname";
            cells["D1"].Formula = "SUM(testname)";

            // Formeln berechnen
            wb.CalculateFormula();

            // Holen Sie den Bereich mit GetRange(true)
            Aspose.Cells.Range namedRange = name.GetRange(true);
            Console.WriteLine($"Named range: FirstRow={namedRange.FirstRow}, FirstColumn={namedRange.FirstColumn}, " +
                $"RowCount={namedRange.RowCount}, ColumnCount={namedRange.ColumnCount}");

            // Erstellen Sie ein Diagramm mit dem benannten Bereich
            int chartIndex = sheet.Charts.Add(ChartType.Column, 10, 1, 20, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("testname", true);
            Console.WriteLine($"Chart data points count: {chart.NSeries[0].CountOfDataValues}");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRange(int, int, int) {#getrange_2}

Liest den Bereich, wenn sich dieser Name auf einen Bereich bezieht. Wenn die Referenz dieses Namens nicht absolut ist, kann der Bereich für verschiedene Zellen unterschiedlich sein.

```csharp
public Range GetRange(int sheetIndex, int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | Int32 | Der entsprechende Blattindex. |
| row | Int32 | Der entsprechende Zeilenindex. |
| column | Int32 | Der entsprechende Spaltenindex |

### Rückgabewert

Der Bereich.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Dairy");
            
            // Erstellen Sie einen benannten Bereich mit der korrekten Methodensignatur
            int index = workbook.Worksheets.Names.Add("SubCat");
            workbook.Worksheets.Names["SubCat"].RefersTo = "=" + worksheet.Name + "!A2:A4";
            
            // Holen Sie den Bereich mit GetRange unter Verwendung von Zeilen-, Spalten- und Zeilenanzahl-Parametern
            Aspose.Cells.Range range = workbook.Worksheets.Names["SubCat"].GetRange(0, 0, 3);
            
            // Zeigen Sie die Bereichsreferenz an
            Console.WriteLine("Range refers to: " + range.RefersTo);
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


