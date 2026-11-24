---
title: "WorkbookSettings.IsProtected"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt einen Wert zurück, der angibt, ob die Struktur oder das Fenster der Arbeitsmappe geschützt ist"
type: docs
url: /de/net/aspose.cells/workbooksettings/isprotected/
---
## WorkbookSettings.IsProtected property

Liest einen Wert, der angibt, ob die Struktur oder das Fenster des Workbooks geschützt ist.

```csharp
public bool IsProtected { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;
            
            // Überprüfen, ob die Arbeitsmappe geschützt ist
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Die Arbeitsmappe mit einem Passwort schützen
            settings.Password = "password123";
            
            // Überprüfen Sie den Schutzstatus
            Console.WriteLine("Workbook is protected: " + settings.IsProtected);
            
            // Speichern Sie die geschützte Arbeitsmappe
            workbook.Save("ProtectedWorkbook.xlsx", SaveFormat.Xlsx);
            
            // Öffnen der geschützten Arbeitsmappe
            Workbook protectedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            
            // Überprüfen des Schutzstatus der geladenen Arbeitsmappe
            Console.WriteLine("Loaded workbook is protected: " + protectedWorkbook.Settings.IsProtected);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


