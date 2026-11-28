---
title: "CellRichValue.ErrorValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellRichValue özelliği. Hücrenin hata değer tipini alır"
type: docs
url: /tr/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

Hücrenin hata değeri tipini alır.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresinde bir spill hatası oluşturun
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // Spill hatasını oluşturmak için formülleri hesaplayın
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Beklenen dökülme hatası
            }
            
            // A1 hücresinden zengin değeri alın
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Hata türünü kontrol edin ve görüntüleyin
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


