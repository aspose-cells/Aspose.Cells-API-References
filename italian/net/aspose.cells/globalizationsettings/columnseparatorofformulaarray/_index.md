---
title: "GlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GlobalizationSettings. Ottiene il separatore per gli elementi nei dati di riga degli array nella formula"
type: docs
url: /it/net/aspose.cells/globalizationsettings/columnseparatorofformulaarray/
---
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property

Ottiene il separatore per gli elementi nei dati di riga dell'array nella formula.

```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate con separatore di colonna sovrascritto
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Visualizza il valore corrente del separatore di colonna
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
                globalizationSettings.ColumnSeparatorOfFormulaArray);

            // Crea una formula di array usando il separatore personalizzato
            Cell cell = worksheet.Cells["A1"];
            cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator

            // Verifica l'archiviazione della formula (mostrerebbe punti e virgola nella stringa della formula reale)
            Console.WriteLine("Stored array formula: " + cell.Formula);

            // Salvare la cartella di lavoro modificata
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ColumnSeparatorOfFormulaArray => ';';
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


