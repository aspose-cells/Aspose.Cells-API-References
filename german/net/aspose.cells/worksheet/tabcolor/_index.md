---
title: "Worksheet.TabColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Stellt die Registerkartenfarbe des Arbeitsblatts dar"
type: docs
url: /de/net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Stellt die Registerkartenfarbe des Arbeitsblatts dar.

```csharp
public Color TabColor { get; set; }
```

### Hinweise

Diese Funktion wird nur in ExcelXP (Excel2002) und späteren Versionen unterstützt. Wenn Sie die Datei im Excel97- oder Excel2000-Format speichern, wird sie weggelassen.

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze die Registerkartenfarbe auf Rot
            worksheet.TabColor = Color.Red;
            Console.WriteLine("Tab color set to: " + worksheet.TabColor);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Lösche die Registerkartenfarbe
            worksheet.TabColor = Color.Empty;
            Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
            
            // Speichere die geänderte Arbeitsmappe
            workbook.Save("output_modified.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


