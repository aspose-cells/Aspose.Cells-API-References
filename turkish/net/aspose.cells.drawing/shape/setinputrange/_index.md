---
title: "Shape.SetInputRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Kontrolü doldurmak için kullanılan aralığı ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

Denetimi doldurmak için kullanılan aralığı ayarlar.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Kontrolü doldurmak için kullanılan aralık. |
| isR1C1 | Boolean | Formülün R1C1 olarak biçimlendirilmesi gerekip gerekmediği. |
| isLocal | Boolean | Formülün yerel ayarlara göre biçimlendirilmesi gerekip gerekmediği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // A1:A10 hücrelerine örnek veri ekleyin
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Bir liste kutusu şekli ekle
            Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);

            // Liste kutusu için giriş aralığını ayarlayın (String, Boolean, Boolean parametrelerini kullanarak)
            listBox.SetInputRange("$A$1:$A$6", false, false);

            // Liste kutusu için bağlanmış hücreyi ayarlayın
            listBox.SetLinkedCell("$A$12", false, true);

            // Çalışma kitabını kaydedin
            workbook.Save("SetInputRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


