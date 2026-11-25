---
title: "GlobalizationSettings.ListSeparator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà GlobalizationSettings. Ottiene il separatore per i parametri di elenco della funzione ...etc"
type: docs
url: /it/net/aspose.cells/globalizationsettings/listseparator/
---
## GlobalizationSettings.ListSeparator property

Ottiene il separatore per l'elenco, i parametri della funzione, ...etc.

```csharp
public virtual char ListSeparator { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con impostazioni di globalizzazione personalizzate
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Visualizza il valore corrente di ListSeparator dalle nostre impostazioni personalizzate
            Console.WriteLine("Current ListSeparator value: " + workbook.Settings.GlobalizationSettings.ListSeparator);

            // Crea una formula utilizzando il separatore di elenco personalizzato
            worksheet.Cells["A1"].Formula = "=CONCATENATE(\"Hello\"; \" World\")";
            worksheet.Cells["A2"].Formula = "=SUM(1;2;3)";

            // Calcola le formule con il separatore personalizzato
            workbook.CalculateFormula();

            // Mostra i risultati del calcolo
            Console.WriteLine("Concatenation result: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Sum result: " + worksheet.Cells["A2"].Value);

            // Salva con le formule utilizzando il separatore di elenco personalizzato
            workbook.Save("ListSeparatorDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ListSeparator => ';';
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


