---
title: "TxtLoadOptions.SeparatorString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions-Eigenschaft. Ruft einen Zeichenkettenwert als Trennzeichen ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells/txtloadoptions/separatorstring/
---
## TxtLoadOptions.SeparatorString property

Liest und setzt einen Zeichenkettenwert als Trennzeichen.

```csharp
public string SeparatorString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze Beispieldaten mit benutzerdefiniertem Trennzeichen
            worksheet.Cells["A1"].PutValue("John&Doe");
            worksheet.Cells["B1"].PutValue("30");
            worksheet.Cells["A2"].PutValue("Jane&Smith");
            worksheet.Cells["B2"].PutValue("25");

            // Speichere mit benutzerdefiniertem Trennzeichen
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = "&";
            workbook.Save("output.csv", saveOptions);

            // Lade mit demselben Trennzeichen
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = "&";
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // Überprüfe die geladenen Daten
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


