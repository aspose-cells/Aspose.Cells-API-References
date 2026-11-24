---
title: "Enum CellValueFormatStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellValueFormatStrategy Enum. Gibt an, wie der Stil für den Zellenwert angewendet wird"
type: docs
url: /de/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

Gibt an, wie der Stil für den Zellwert angewendet wird.

```csharp
public enum CellValueFormatStrategy
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Nicht formatiert. |
| CellStyle | `1` | Nur mit dem ursprünglichen Stil der Zelle formatiert. |
| DisplayStyle | `2` | Mit dem angezeigten Stil der Zelle formatiert. |
| DisplayString | `3` | Liefert die in MS Excel angezeigte Zeichenkette. Der Hauptunterschied zu DisplayStyle besteht darin, dass diese Option auch die Auswirkung der Spaltenbreite berücksichtigt. Ist die Spaltenbreite zu klein, um die formatierte Zeichenkette vollständig anzuzeigen, kann \"#\" angezeigt werden, genau wie in MS Excel. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueFormatStrategyDemo
    {
        public static void CellValueFormatStrategyExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Number");
            worksheet.Cells["B2"].PutValue(12345.6789);
            worksheet.Cells["C1"].PutValue("Text");
            worksheet.Cells["C2"].PutValue("Hello World");

            // Wenden Sie verschiedene CellValueFormatStrategy an, um deren Auswirkungen zu demonstrieren
            // None: Nicht formatiert
            string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($"None: {valueNone}");

            // CellStyle: Nur mit dem ursprünglichen Stil der Zelle formatiert
            string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($"CellStyle: {valueCellStyle}");

            // DisplayStyle: Mit dem angezeigten Stil der Zelle formatiert
            string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");

            // DisplayString: Liefert die in MS Excel angezeigte Zeichenkette
            string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($"DisplayString: {valueDisplayString}");

            // Speichere die Arbeitsmappe in einer Datei
            workbook.Save("CellValueFormatStrategyExample.xlsx");
            workbook.Save("CellValueFormatStrategyExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


