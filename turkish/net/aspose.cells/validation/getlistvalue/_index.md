---
title: "Validation.GetListValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Validation yöntemi. Belirtilen hücre için doğrulamanın listesinin değerini al"
type: docs
url: /tr/net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Belirtilen hücre için doğrulama listesinin değerini al.

```csharp
public object GetListValue(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |

### Dönüş Değeri

Belirtilen hücre için bu doğrulamanın listesini üretmek üzere değer. Liste bir aralığa referans veriyorsa, döndürülen değer bir [`ReferredArea`](../../referredarea/) nesnesi olur; aksi takdirde döndürülen değer null, object[] ya da basit bir nesne olabilir.

### Açıklamalar

Yalnızca türü List olan ve verilen hücreye uygulanmış doğrulama için, aksi takdirde null döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetListValueWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğrulama için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");

            // B1 hücresi için doğrulama oluştur
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:A4";

            // Farklı parametrelerle GetListValue test et
            Console.WriteLine("List values:");
            for (int i = 0; i < 4; i++)
            {
                object value = validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {value}");
            }

            // Virgülle ayrılmış değerlere değiştir
            validation.Formula1 = "Red,Green,Blue";
            Console.WriteLine("\nComma-separated values:");
            for (int i = 0; i < 3; i++)
            {
                object[] values = (object[])validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
            }

            // Tek değere değiştir
            validation.Formula1 = "SingleValue";
            Console.WriteLine("\nSingle value:");
            object singleValue = validation.GetListValue(0, 0);
            Console.WriteLine($"Value: {singleValue}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


