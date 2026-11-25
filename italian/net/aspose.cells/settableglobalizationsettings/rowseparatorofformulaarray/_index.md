---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SettableGlobalizationSettings. Ottiene il separatore per le righe nei dati dell'array nella formula"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

Ottiene il separatore per le righe nei dati dell'array nella formula.

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Visualizza il separatore di riga predefinito per gli array di formule
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Imposta un nuovo separatore di riga per gli array di formule
            settings.SetRowSeparatorOfFormulaArray(';');

            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            // Crea una formula di array nel foglio di lavoro
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // Calcola le formule
            workbook.CalculateFormula();

            // Salva la cartella di lavoro
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


