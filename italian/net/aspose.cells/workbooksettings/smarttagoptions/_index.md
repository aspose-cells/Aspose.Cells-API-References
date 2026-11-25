---
title: "WorkbookSettings.SmartTagOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene le opzioni del tag intelligente"
type: docs
url: /it/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

Ottiene le opzioni del tag intelligente.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();

                // Accedi alle impostazioni della cartella di lavoro
                WorkbookSettings settings = workbook.Settings;

                // Leggi la proprietà SmartTagOptions
                var smartTagOptions = settings.SmartTagOptions;

                // Visualizza le informazioni sull'istanza di SmartTagOptions
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // Facoltativamente, puoi ispezionare lo stato predefinito tramite ToString()
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // Salva la cartella di lavoro (il file conterrà le impostazioni predefinite)
                workbook.Save("SmartTagOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


