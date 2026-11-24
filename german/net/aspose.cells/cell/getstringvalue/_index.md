---
title: "Cell.GetStringValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt den Zeichenkettenwert anhand einer spezifischen Formatierungsstrategie zurück"
type: docs
url: /de/net/aspose.cells/cell/getstringvalue/
---
## Cell.GetStringValue method

Liefert den Zeichenkettenwert nach einer spezifischen Formatierungsstrategie.

```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | Die formatierte Strategie. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStringValueWithCellValueFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Verschiedene Datentypen in Zellen festlegen
            cells["A1"].PutValue(123.45); // Numeric value
            cells["A2"].PutValue(DateTime.Now); // DateTime value
            cells["A3"].PutValue(true); // Boolean value
            cells["A4"].PutValue("Sample Text"); // String value

            // Demonstriere GetStringValue mit verschiedenen Formatstrategien
            Console.WriteLine("None: " + cells["A1"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("CellStyle: " + cells["A1"].GetStringValue(CellValueFormatStrategy.CellStyle));
            Console.WriteLine("DisplayString: " + cells["A1"].GetStringValue(CellValueFormatStrategy.DisplayString));

            Console.WriteLine("DateTime None: " + cells["A2"].GetStringValue(CellValueFormatStrategy.None));
            Console.WriteLine("DateTime CellStyle: " + cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle));
        }
    }
}
```

### Siehe auch

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


