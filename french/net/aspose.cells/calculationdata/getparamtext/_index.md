---
title: "CalculationData.GetParamText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CalculationData. Obtient le texte littéral du paramètre à l'index donné"
type: docs
url: /fr/net/aspose.cells/calculationdata/getparamtext/
---
## CalculationData.GetParamText method

Obtient le texte littéral du paramètre à l'index donné.

```csharp
public string GetParamText(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | index du paramètre (base 0) |

### Valeur de retour

texte littéral du paramètre

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamTextWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            sheet.Cells["A1"].Formula = "=SUM(INDIRECT(\"'Book2.xlsx'!Table1[#All]\"))";
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();
            workbook.CalculateFormula(options);
        }
    }

    class CustomCalcEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                Console.WriteLine("SUM parameter: " + data.GetParamText(0));
            }
            else if (data.FunctionName == "INDIRECT")
            {
                Console.WriteLine("INDIRECT parameter: " + data.GetParamText(0));
            }
        }
    }
}
```

### Voir aussi

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


