---
title: "WorkbookSettings.EnableMacros"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Abilita le macro"
type: docs
url: /it/net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

Abilita le macro;

```csharp
public bool EnableMacros { get; set; }
```

### Osservazioni

Ora funziona solo quando si copia un foglio di lavoro in un altro foglio di lavoro all'interno di una cartella di lavoro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyEnableMacrosDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = wb.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Macro Test");
            
            // Dimostra la proprietà EnableMacros
            Console.WriteLine("Initial EnableMacros value: " + wb.Settings.EnableMacros);
            
            // Disabilita le macro
            wb.Settings.EnableMacros = false;
            Console.WriteLine("After disabling macros: " + wb.Settings.EnableMacros);
            
            // Abilita le macro
            wb.Settings.EnableMacros = true;
            Console.WriteLine("After enabling macros: " + wb.Settings.EnableMacros);
            
            // Salva la cartella di lavoro
            wb.Save("EnableMacrosDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


