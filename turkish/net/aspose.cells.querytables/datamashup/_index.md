---
title: "Sınıf DataMashup"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.QueryTables.DataMashup sınıfı. Mashup verilerini temsil eder"
type: docs
url: /tr/net/aspose.cells.querytables/datamashup/
---
## DataMashup class

Karışım verisini temsil eder.

```csharp
public class DataMashup
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**Obsolete.**) Power query formül parametrelerini alır. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | Tüm power query formüllerini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class DataMashupDemo
    {
        public static void DataMashupExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabının DataMashup özelliğine eriş
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // PowerQueryFormulas özelliğine eriş
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // PowerQueryFormulaParameters özelliğine eriş
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Örnek kullanım: PowerQueryFormulas üzerinden yinele
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Örnek kullanım: PowerQueryFormulaParameters üzerinden yineleyin
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // Çalışma kitabını kaydedin
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


