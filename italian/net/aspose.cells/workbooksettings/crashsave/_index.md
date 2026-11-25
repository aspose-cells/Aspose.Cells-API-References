---
title: "WorkbookSettings.CrashSave"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. indica se l'applicazione ha salvato l'ultimo file cartella di lavoro dopo un arresto anomalo"
type: docs
url: /it/net/aspose.cells/workbooksettings/crashsave/
---
## WorkbookSettings.CrashSave property

Indica se l'applicazione ha salvato l'ultimo file workbook dopo un arresto anomalo.

```csharp
public bool CrashSave { get; set; }
```

### Esempi

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCrashSaveDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("CrashSave Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Dimostra la proprietà CrashSave
            settings.CrashSave = true;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Salva con il salvataggio di emergenza abilitato
            workbook.Save("CrashSaveEnabled.xlsx");

            // Disabilita il salvataggio di emergenza
            settings.CrashSave = false;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Salva con il salvataggio di emergenza disabilitato
            workbook.Save("CrashSaveDisabled.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


