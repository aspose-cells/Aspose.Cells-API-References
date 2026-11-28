---
title: "FindOptions.LookInType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Arama türü"
type: docs
url: /tr/net/aspose.cells/findoptions/lookintype/
---
## FindOptions.LookInType property

Tür içinde bak.

```csharp
public LookInType LookInType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookInTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve örnek veri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelerdeki değerleri ve formülleri ayarla
            worksheet.Cells["A1"].PutValue("SearchValue");
            worksheet.Cells["A2"].Formula = "=A1";
            worksheet.Cells["B1"].PutValue("OtherValue");

            // Yalnızca formüllerde arama yapmak için bulma seçenekleri oluştur
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            // Formüllerdeki değeri ara
            Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);

            // Sonucu çıktı olarak ver
            if (foundCell != null)
            {
                Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
            }
            else
            {
                Console.WriteLine("Value not found in formulas");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


