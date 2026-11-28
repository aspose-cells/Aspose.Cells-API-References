---
title: "PowerQueryFormulaFunction.F"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormulaFunction özelliği. Fonksiyon tanımını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

İşlevin tanımını alır ve ayarlar.

```csharp
public string F { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaFunctionPropertyFDemo
    {
        public static void Run()
        {
            // Mevcut Power Query formüllerini içeren bir çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsx");
            
            // Power Query formülleri koleksiyonuna eriş
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Adına göre mevcut bir fonksiyon formülünü al
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // F özelliğine erişmek için PowerQueryFormulaFunction'a dönüştürün
            if (formula is PowerQueryFormulaFunction function)
            {
                // F özelliğini almayı gösterin
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // F özelliğini ayarlamayı gösterin
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


