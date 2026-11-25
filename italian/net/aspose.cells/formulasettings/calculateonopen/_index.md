---
title: "FormulaSettings.CalculateOnOpen"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FormulaSettings. Indica se l'applicazione è tenuta a eseguire un calcolo completo quando la cartella di lavoro viene aperta"
type: docs
url: /it/net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Indica se l'applicazione deve eseguire un calcolo completo quando la cartella di lavoro viene aperta.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Osservazioni

Questa proprietà serve solo a salvare le impostazioni nel file di foglio di calcolo risultante in modo che altre applicazioni (come MS Excel) possano comportarsi di conseguenza al caricamento del file risultante. Per motivi di prestazioni nella maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro, indipendentemente dal valore impostato per questa proprietà.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnOpenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la formula nella cella A1 che fa riferimento a B1
            worksheet.Cells["A1"].Formula = "=B1";
            
            // Imposta il valore nella cella B1
            worksheet.Cells["B1"].PutValue(10);
            
            // Disabilita il calcolo automatico delle formule all'apertura
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Riapri la cartella di lavoro salvata
            Workbook reopenedWorkbook = new Workbook("output.xlsx");
            
            // Verifica che la formula non sia stata calcolata all'apertura
            Console.WriteLine("A1 value (should be 0 before calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
            
            // Calcola le formule manualmente
            reopenedWorkbook.CalculateFormula();
            
            // Verifica che la formula sia stata calcolata
            Console.WriteLine("A1 value (should be 10 after calculation): " + reopenedWorkbook.Worksheets[0].Cells["A1"].IntValue);
        }
    }
}
```

### Vedi anche

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


