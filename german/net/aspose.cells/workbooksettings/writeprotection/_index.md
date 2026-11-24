---
title: "WorkbookSettings.WriteProtection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Bietet Zugriff auf die Schreibschutzoptionen der Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/workbooksettings/writeprotection/
---
## WorkbookSettings.WriteProtection property

Stellt Zugriff auf die Schreibschutzoptionen der Arbeitsmappe bereit.

```csharp
public WriteProtection WriteProtection { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWriteProtectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Setze Schreibschutz-Eigenschaften
            workbook.Settings.WriteProtection.Password = "test123";
            workbook.Settings.WriteProtection.Author = "John Doe";
            workbook.Settings.WriteProtection.RecommendReadOnly = true;

            // Speichere die Arbeitsmappe
            string outputPath = "WriteProtectionDemo.xlsx";
            workbook.Save(outputPath);

            // Laden der gespeicherten Arbeitsmappe, um Eigenschaften zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Gib die Schreibschutz-Eigenschaften aus
            Console.WriteLine("Author: " + loadedWorkbook.Settings.WriteProtection.Author);
            Console.WriteLine("ReadOnly Recommended: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
        }
    }
}
```

### Siehe auch

* class [WriteProtection](../../writeprotection/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


