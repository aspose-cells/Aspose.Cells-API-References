---
title: "WorkbookSettings.BuildVersion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Specifica la versione pubblica incrementale dell'applicazione"
type: docs
url: /it/net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

Specifica la versione incrementale pubblica dell'applicazione.

```csharp
public string BuildVersion { get; set; }
```

### Esempi

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyBuildVersionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi a WorkbookSettings
            WorkbookSettings settings = workbook.Settings;
            
            // Imposta le impostazioni di base
            settings.Author = "Sample Author";
            settings.CultureInfo = new CultureInfo("en-US");
            
            // Dimostra la proprietà BuildVersion
            settings.BuildVersion = "2.5.0";
            Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
            
            // Salva la cartella di lavoro
            workbook.Save("BuildVersionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


