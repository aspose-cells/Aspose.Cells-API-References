---
title: "PowerQueryFormula.PowerQueryFormulaItems"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PowerQueryFormula özelliği. Power query formülünün tüm öğelerini alır"
type: docs
url: /tr/net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Power query formülünün tüm öğelerini alır.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyPowerQueryFormulaItemsDemo
    {
        public static void Run()
        {
            // Kaynak çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsx");

            // İlk Power Query formülüne ve onun ilk öğesine erişin
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            
            // Öğe değerini değiştirin (sürücü harfini değiştirin)
            string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
            item.Value = modifiedValue;

            // Çalışma kitabını kaydedin
            workbook.Save("modified_example.xlsx");

            // Değişikliği doğrulayın
            Console.WriteLine("Original value modified to: " + modifiedValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


