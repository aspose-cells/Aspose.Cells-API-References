---
title: "WorkbookSettings.Shared"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob das Arbeitsbuch freigegeben ist"
type: docs
url: /de/net/aspose.cells/workbooksettings/shared/
---
## WorkbookSettings.Shared property

Liest oder setzt einen Wert, der angibt, ob die Arbeitsmappe freigegeben ist.

```csharp
public bool Shared { get; set; }
```

### Hinweise

Der Standardwert ist false.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySharedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook book = new Workbook();
            
            // Setze die Shared-Eigenschaft auf true
            book.Settings.Shared = true;
            
            // Speichere die Arbeitsmappe
            string outputPath = "output_shared.xlsx";
            book.Save(outputPath);
            
            // Lade das gespeicherte Arbeitsbuch, um die Shared-Eigenschaft zu überprüfen
            Workbook loadedBook = new Workbook(outputPath);
            Console.WriteLine("Shared property value: " + loadedBook.Settings.Shared);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


