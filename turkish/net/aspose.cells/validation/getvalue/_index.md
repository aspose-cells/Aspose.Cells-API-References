---
title: "Validation.GetValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama yöntemi. Belirli hücredeki doğrulama değerini al"
type: docs
url: /tr/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

Belirli hücredeki doğrulamanın değerini al.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |
| isValue1 | Boolean | İlk değerin alınıp alınmadığını gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ve doğrulama ekle
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // B1 hücresi için doğrulama oluştur
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // Satır, sütun ve sayısal değeri tarihe dönüştür parametreleriyle GetValue yöntemini kullanarak değeri al
            object value = validation.GetValue(0, 1, false);
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


