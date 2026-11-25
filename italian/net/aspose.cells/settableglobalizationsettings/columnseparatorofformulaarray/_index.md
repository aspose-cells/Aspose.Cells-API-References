---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SettableGlobalizationSettings. Ottiene il separatore per gli elementi nei dati di riga degli array nella formula"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

Ottiene il separatore per gli elementi nei dati di riga dell'array nella formula.

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Visualizza il valore corrente di ColumnSeparatorOfFormulaArray
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // Imposta un nuovo valore per ColumnSeparatorOfFormulaArray
            settings.SetColumnSeparatorOfFormulaArray(';');

            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            // Crea una formula di matrice con il separatore personalizzato usando SetArrayFormula
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // Calcola le formule
            workbook.CalculateFormula();

            // Visualizza il risultato
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // Salva la cartella di lavoro
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


