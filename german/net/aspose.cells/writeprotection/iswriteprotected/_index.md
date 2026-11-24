---
title: "WriteProtection.IsWriteProtected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WriteProtection-Eigenschaft. Gibt an, ob diese Arbeitsmappe schreibgeschützt ist"
type: docs
url: /de/net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Gibt an, ob diese Arbeitsmappe schreibgeschützt ist.

```csharp
public bool IsWriteProtected { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyIsWriteProtectedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Schreibschutz mit Passwort aktivieren
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Prüfe, ob die Arbeitsmappe schreibgeschützt ist
            Console.WriteLine("Is workbook write protected? " + 
                workbook.Settings.WriteProtection.IsWriteProtected);
            
            // Das Passwort validieren
            Console.WriteLine("Is password valid? " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            
            // Speichere die Arbeitsmappe
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            // Lade die gespeicherte Arbeitsmappe, um den Schutz zu überprüfen
            Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
            
            // Schutzstatus erneut prüfen
            Console.WriteLine("Is loaded workbook write protected? " + 
                loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Siehe auch

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


