---
title: "AutoFilter.ShowAll"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Alle Zeilen einblenden"
type: docs
url: /de/net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

Alle Zeilen einblenden.

```csharp
public void ShowAll()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodShowAllDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // Auto-Filter anwenden
            worksheet.AutoFilter.Range = "A1:A5";
            
            // Filter, um nur "Apple" anzuzeigen
            worksheet.AutoFilter.Filter(0, "Apple");
            
            // Alle Daten wieder anzeigen
            worksheet.AutoFilter.ShowAll();
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


