---
title: "CalculationOptions.CalculationMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. Il monitor per l'utente per tenere traccia dell'avanzamento del calcolo delle formule"
type: docs
url: /it/net/aspose.cells/calculationoptions/calculationmonitor/
---
## CalculationOptions.CalculationMonitor property

Il monitor per l'utente per tracciare l'avanzamento del calcolo delle formule.

```csharp
public AbstractCalculationMonitor CalculationMonitor { get; set; }
```

### Esempi

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalculationMonitorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcune formule di esempio
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Crea opzioni di calcolo con un monitor personalizzato
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new SampleCalculationMonitor();

            // Calcola le formule con monitoraggio
            workbook.CalculateFormula(options);

            // Restituisci i risultati
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("A2: " + worksheet.Cells["A2"].Value);
            Console.WriteLine("A3: " + worksheet.Cells["A3"].Value);
        }
    }

    public class SampleCalculationMonitor : AbstractCalculationMonitor
    {
        public override bool OnCircular(IEnumerator circularCellsData)
        {
            // Gestisci i riferimenti circolari se necessario
            return base.OnCircular(circularCellsData);
        }

        public override void BeforeCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Before calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"After calculation: Sheet{sheetIndex}, Row{rowIndex}, Col{columnIndex}");
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


