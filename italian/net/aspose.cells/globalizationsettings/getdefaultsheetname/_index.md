---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome del foglio predefinito per l'aggiunta automatica di un foglio di lavoro. Il valore predefinito è Sheet"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

Ottiene il nome del foglio predefinito per l'aggiunta automatica del foglio di lavoro. Il valore predefinito è "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### Valore di ritorno

Il nome predefinito del foglio per l'aggiunta automatica di un foglio di lavoro

### Osservazioni

Il nome del foglio aggiunto automaticamente (ad esempio tramite [`Add`](../../worksheetcollection/add/)) sarà il nome specificato più un numero di sequenza. Per esempio, per un utente tedesco potrebbe voler che il nome del foglio sia "Tabellenblatt2" invece di "Sheet2". L'utente può quindi implementare questo metodo per restituire "Tabellenblatt".

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta impostazioni di globalizzazione personalizzate
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Ottieni il nome predefinito del foglio dalle impostazioni di globalizzazione personalizzate
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // Aggiungi un nuovo foglio di lavoro per dimostrare la denominazione basata sul valore predefinito personalizzato
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // Implementazione delle impostazioni di globalizzazione personalizzate
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


