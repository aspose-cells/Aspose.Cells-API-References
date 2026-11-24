---
title: "Worksheet.CodeName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet‑Eigenschaft. Gibt den CodeName des Arbeitsblatts zurück"
type: docs
url: /de/net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Liest den Code-Namen des Arbeitsblatts.

```csharp
public string CodeName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCodeNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zeigen Sie den Standard‑CodeName an
            Console.WriteLine("Default CodeName: " + worksheet.CodeName);
            
            // Ändern Sie den CodeName
            worksheet.CodeName = "MySheet";
            Console.WriteLine("Modified CodeName: " + worksheet.CodeName);
            
            // Fügen Sie ein neues Arbeitsblatt hinzu und zeigen Sie dessen CodeName an
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            Console.WriteLine("New Sheet CodeName: " + newSheet.CodeName);
            
            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetCodeNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


