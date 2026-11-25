---
title: "SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Restituisce il testo dell'intestazione del campo dell'area valori nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader method

Restituisce il testo dell'intestazione del campo dell'area valori nella PivotTable.

```csharp
public override string GetTextOfDataFieldHeader()
```

### Valore di ritorno

Il testo del nome dell'intestazione del campo dati

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfDataFieldHeaderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per il contesto
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Crea un'istanza di SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ottieni il testo predefinito per l'intestazione del campo dati
                string dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Default data field header text: {dataFieldHeaderText}");

                // Imposta un testo personalizzato per l'intestazione del campo dati
                settings.SetTextOfDataFieldHeader("Custom Data Header");
                dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Updated data field header text: {dataFieldHeaderText}");

                // Salva la cartella di lavoro
                workbook.Save("GetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("GetTextOfDataFieldHeader method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


