---
title: "WorkbookSettings.Password"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WorkbookSettings property. Rappresenta la password di crittografia del file della cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/password/
---
## WorkbookSettings.Password property

Rappresenta la password di crittografia del file Workbook.

```csharp
public string Password { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["C6"].PutValue("test encrypt.");
            
            // Imposta la password per proteggere la cartella di lavoro
            wb.Settings.Password = "xixi";
            
            // Salva la cartella di lavoro
            wb.Save("output_with_password.ods");
            
            // Crea le opzioni di caricamento con password per aprire la cartella di lavoro protetta
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "xixi";
            
            // Apri la cartella di lavoro protetta da password
            Workbook wbProtected = new Workbook("output_with_password.ods", loadOptions);
            
            // Verifica i dati
            Console.WriteLine("Cell value: " + wbProtected.Worksheets[0].Cells["C6"].Value);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


