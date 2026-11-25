---
title: "WorkbookSettings.RemovePersonalInformation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. True se le informazioni personali possono essere rimosse dalla cartella di lavoro specificata"
type: docs
url: /it/net/aspose.cells/workbooksettings/removepersonalinformation/
---
## WorkbookSettings.RemovePersonalInformation property

Vero se le informazioni personali possono essere rimosse dal workbook specificato.

```csharp
public bool RemovePersonalInformation { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta RemovePersonalInformation a true
            workbook.Settings.RemovePersonalInformation = true;
            
            // Aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Email");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue("john@example.com");
            
            // Salva la cartella di lavoro
            string outputPath = "output_with_personal_info_removed.xlsx";
            workbook.Save(outputPath);
            
            // Carica la cartella di lavoro salvata per verificare l'impostazione
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("RemovePersonalInformation setting: " + 
                loadedWorkbook.Settings.RemovePersonalInformation);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


