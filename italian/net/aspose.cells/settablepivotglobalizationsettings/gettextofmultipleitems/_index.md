---
title: "SettablePivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettablePivotGlobalizationSettings. Ottiene il testo dell'etichetta Multiple Items nella PivotTable"
type: docs
url: /it/net/aspose.cells/settablepivotglobalizationsettings/gettextofmultipleitems/
---
## SettablePivotGlobalizationSettings.GetTextOfMultipleItems method

Restituisce il testo dell'etichetta "(Multiple Items)" nella PivotTable.

```csharp
public override string GetTextOfMultipleItems()
```

### Valore di ritorno

Il testo dell'etichetta "(Multiple Items)"

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
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
                // Ottieni il testo predefinito per più elementi
                string multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Default text for multiple items: {multipleItemsText}");

                // Imposta un testo personalizzato per più elementi
                settings.SetTextOfMultipleItems("(Multiple Items Custom)");
                multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Updated text for multiple items: {multipleItemsText}");

                // Salva la cartella di lavoro
                workbook.Save("GetTextOfMultipleItemsDemo.xlsx");
                Console.WriteLine("GetTextOfMultipleItems method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


