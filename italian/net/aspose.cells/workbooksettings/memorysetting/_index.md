---
title: "WorkbookSettings.MemorySetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene o imposta le opzioni di utilizzo della memoria. La nuova opzione sarà presa come predefinita per i fogli di lavoro appena creati, ma non avrà effetto sui fogli di lavoro esistenti"
type: docs
url: /it/net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Ottiene o imposta le opzioni di utilizzo della memoria. La nuova opzione sarà presa come opzione predefinita per i fogli di lavoro appena creati, ma non avrà effetto sui fogli di lavoro esistenti.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Osservazioni

Per ulteriori dettagli sulla modalità di memoria, consulta [`MemorySetting`](../../cells/memorysetting/).

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con l'impostazione di preferenza della memoria
            Workbook wb = new Workbook();
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            
            // Accedi al primo foglio di lavoro e aggiungi alcuni dati
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Memory Setting Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Salva in un flusso di memoria con formato PDF
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Pdf);
                Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
            }
        }
    }
}
```

### Vedi anche

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


