---
title: "DataMashup.PowerQueryFormulaParameters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataMashup özelliği. Power query formül parametrelerini alır"
type: docs
url: /tr/net/aspose.cells.querytables/datamashup/powerqueryformulaparameters/
---
## DataMashup.PowerQueryFormulaParameters property

Power query formül parametrelerini alır.

```csharp
[Obsolete("Use DataMashup.PowerQueryFormulas property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PowerQueryFormulaParameterCollection PowerQueryFormulaParameters { get; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine, lütfen DataMashup.PowerQueryFormulas özelliğini kullanın. Bu özellik Kasım 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class DataMashupPropertyPowerQueryFormulaParametersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // DataMashup özelliğine erişin
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null)
            {
                // PowerQueryFormulaParameters'a erişin
                PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                // Parametre sayısını göster
                Console.WriteLine($"Number of parameters: {parameters.Count}");

                // Varsa parametreler üzerinden yineleyin
                foreach (PowerQueryFormulaParameter parameter in parameters)
                {
                    Console.WriteLine($"Parameter Name: {parameter.Name}, Value: {parameter.Value}");
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("DataMashupDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormulaParameterCollection](../../powerqueryformulaparametercollection/)
* class [DataMashup](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


