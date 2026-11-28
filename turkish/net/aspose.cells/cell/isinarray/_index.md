---
title: "Cell.IsInArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücre formülünün bir dizi formülü olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cell/isinarray/
---
## Cell.IsInArray property

Hücre formülünün bir dizi formülü olup olmadığını gösterir.

```csharp
[Obsolete("Use IsArrayFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInArray { get; }
```

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine, hücre formülünün bir dizi formülü olup olmadığını kontrol etmek için lütfen Cell.IsArrayFormula kullanın. Bu özellik Mayıs 2018'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsInArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dizi formülleriyle örnek veri oluşturun
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Doğru API'yi kullanarak bir dizi formülü ayarlayın
            worksheet.Cells["C2"].SetArrayFormula("A2:A3*B2:B3", 2, 1);

            // IsInArray özelliğini kontrol edin
            Cell cellInArray = worksheet.Cells["C2"];
            Cell cellNotInArray = worksheet.Cells["A2"];

            Console.WriteLine("Cell C2 is in array: " + cellInArray.IsInArray);
            Console.WriteLine("Cell A2 is in array: " + cellNotInArray.IsInArray);

            // Dizi olmayan hücreleri temizlemeyi gösterin
            for (int row = 1; row <= 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = worksheet.Cells[row, col];
                    if (!cell.IsInArray && !cell.IsFormula)
                    {
                        cell.PutValue("");
                    }
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("IsInArrayDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


