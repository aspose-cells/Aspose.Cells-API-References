---
title: "SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Imposta il separatore per le righe nei dati dell'array nella formula"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray method

Imposta il separatore per le righe nei dati dell'array nella formula.

```csharp
public void SetRowSeparatorOfFormulaArray(char c)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| c | Carattere | il separatore specificato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Imposta il separatore di riga per gli array di formula a '|'
            char rowSeparator = '|';
            settings.SetRowSeparatorOfFormulaArray(rowSeparator);

            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            // Crea una formula di array nel foglio di lavoro
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            
            try
            {
                // Calcola la formula per applicare le impostazioni
                workbook.CalculateFormula();

                // Visualizza la formula con il nuovo separatore di riga
                Console.WriteLine("Array formula with custom row separator: " + worksheet.Cells["A1"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRowSeparatorOfFormulaArray method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("MethodSetRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


