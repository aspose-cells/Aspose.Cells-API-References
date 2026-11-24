---
title: "Workbook.RemovePersonalInformation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Entfernt persönliche Informationen"
type: docs
url: /de/net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Entfernt persönliche Informationen.

```csharp
public void RemovePersonalInformation()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Einen Kommentar mit Autoreninformationen hinzufügen
            int commentIndex = sheet.Comments.Add("A1");
            sheet.Comments[commentIndex].Note = "Sample comment";
            sheet.Comments[commentIndex].Author = "Test Author";
            
            // Ursprüngliche Autoreninformationen anzeigen
            Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
            
            // Persönliche Informationen entfernen
            wb.RemovePersonalInformation();
            
            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Neu laden, um die Entfernung zu überprüfen
            Workbook wb2 = new Workbook("output.xlsx");
            Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


