---
title: "GlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GlobalizationSettings. Ottiene il separatore per le righe nei dati dell'array nella formula"
type: docs
url: /it/net/aspose.cells/globalizationsettings/rowseparatorofformulaarray/
---
## GlobalizationSettings.RowSeparatorOfFormulaArray property

Ottiene il separatore per le righe nei dati dell'array nella formula.

```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con impostazioni di globalizzazione personalizzate
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi all'istanza delle impostazioni di globalizzazione personalizzate
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            // Visualizza il valore corrente di RowSeparatorOfFormulaArray
            Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Crea una formula di matrice utilizzando il separatore di riga personalizzato
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator

            // Calcola la formula per dimostrare il corretto parsing
            workbook.CalculateFormula();

            // Visualizza i risultati
            Console.WriteLine("Array formula using custom separator: " + cell.Formula);
            Console.WriteLine("Calculated result: " + cell.Value);

            // Salva la cartella di lavoro
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }

    // Implementazione personalizzata di GlobalizationSettings che sovrascrive il separatore di riga
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override char RowSeparatorOfFormulaArray => '|';
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


