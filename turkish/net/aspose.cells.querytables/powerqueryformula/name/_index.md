---
title: "PowerQueryFormula.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormula özelliği. Power query formülünün adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Power query formülünün adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Power Query formülleri içeren mevcut bir dosyayı yükle
            workbook = new Workbook("example.xlsx");
            
            // Mevcut Power Query formüllerine erişin
            if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
            {
                PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
                
                // Name özelliğinin kullanımını göster
                Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
                
                // Adı değiştir
                formula.Name = "UpdatedSalesFilter";
                Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
                
                // Çalışma kitabını kaydedin
                workbook.Save("PowerQueryFormulaDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


