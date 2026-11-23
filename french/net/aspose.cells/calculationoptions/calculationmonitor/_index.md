---
title: "CalculationOptions.CalculationMonitor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. Le moniteur pour l'utilisateur afin de suivre la progression du calcul de formule"
type: docs
url: /fr/net/aspose.cells/calculationoptions/calculationmonitor/
---
## CalculationOptions.CalculationMonitor property

Le moniteur permettant à l'utilisateur de suivre la progression du calcul des formules.

```csharp
public AbstractCalculationMonitor CalculationMonitor { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir quelques formules d'exemple
            worksheet.Cells["A1"].Formula = "=1+2";
            worksheet.Cells["A2"].Formula = "=A1*3";
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Créer des options de calcul avec un moniteur personnalisé
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new SampleCalculationMonitor();

            // Calculer les formules avec surveillance
            workbook.CalculateFormula(options);

            // Afficher les résultats
            Console.WriteLine("A1: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("A2: " + worksheet.Cells["A2"].Value);
            Console.WriteLine("A3: " + worksheet.Cells["A3"].Value);
        }
    }

    public class SampleCalculationMonitor : AbstractCalculationMonitor
    {
        public override bool OnCircular(IEnumerator circularCellsData)
        {
            // Gérer les références circulaires si nécessaire
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

### Voir aussi

* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


