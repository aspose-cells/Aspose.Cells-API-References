---
title: "PowerQueryFormula.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormula özelliği. Bu power query formülünün tipini alır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

Bu power query formülünün tipini alır.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Mevcut formülleri al (yeni çalışma kitabında yok) Type özelliğini göstermek için
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Gerçek bir senaryoda mevcut formüllerle, tiplerini kontrol ederiz
            Console.WriteLine("Power Query Formula Types:");
            
            // Bu, Type özelliğini kontrol etmeyi gösterir
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // Demonstrasyon amaçları için, formül yokken çıktı ekle
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


