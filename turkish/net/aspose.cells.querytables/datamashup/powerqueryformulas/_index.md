---
title: "DataMashup.PowerQueryFormulas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataMashup özelliği. Tüm power query formüllerini alır"
type: docs
url: /tr/net/aspose.cells.querytables/datamashup/powerqueryformulas/
---
## DataMashup.PowerQueryFormulas property

Tüm power query formüllerini alır.

```csharp
public PowerQueryFormulaCollection PowerQueryFormulas { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulasDemo
    {
        public static void Run()
        {
            // Power Query formülleriyle çalışma kitabını yükle
            Workbook workbook = new Workbook("source.xlsx");
            
            // DataMashup nesnesini al
            DataMashup mashupData = workbook.DataMashup;
            
            // Power Query formüllerinin olup olmadığını kontrol edin
            if (mashupData != null && mashupData.PowerQueryFormulas != null)
            {
                Console.WriteLine("Power Query Formulas Found:");
                
                // Her bir Power Query formülünü yineleyin
                foreach (PowerQueryFormula formula in mashupData.PowerQueryFormulas)
                {
                    Console.WriteLine("Formula Definition:");
                    Console.WriteLine(formula.FormulaDefinition);
                    Console.WriteLine("----------------------");
                }
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormulaCollection](../../powerqueryformulacollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


