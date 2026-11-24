---
title: "PivotItem.GetStringValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotItem-Methode. Gibt den Zeichenkettenwert des Pivot-Elements zurück. Wenn der Wert null ist, wird zurückgegeben"
type: docs
url: /de/net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Ermittelt den Zeichenkettenwert des Pivot-Elements. Wenn der Wert null ist, wird "" zurückgegeben.

```csharp
public string GetStringValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetStringValueDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("example.xlsx");
            
            // Greifen Sie auf das erste Arbeitsblatt und die Pivot-Tabelle zu
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Holen Sie das erste Zeilenfeld und seine Pivot-Elemente
            PivotField rowField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = rowField.PivotItems;
            
            // Demonstrieren Sie die Methode GetStringValue()
            string itemValue = pivotItems[1].GetStringValue();
            Console.WriteLine("PivotItem value: " + itemValue);
            
            // Speichere die geänderte Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


