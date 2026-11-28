---
title: "Sınıf GroupFill"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.GroupFill class. Bu dolgu formatının grubun dolgu özelliklerini miras alması gerektiğini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Bu doldurma biçiminin grupun doldurma özelliklerini devralması gerektiğini temsil eder.

```csharp
public class GroupFill : Fill
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Şuradan [`Fill`](../fill/) devralınmıştır.) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Karma kodu alır. (Şuradan [`Fill`](../fill/) devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill, parametresiz bir public yapıcıyı ortaya çıkarmaz.
                // Demonstrasyon amacıyla tipin bir referansını (null) elde ederiz.
                GroupFill groupFill = null;

                // GroupFill tipindeki değişkenin mevcut olduğunu gösterin.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // Çalışma kitabını kaydedin (değiştirmemiş olsak da, bu tam bir iş akışını gösterir)
                workbook.Save("GroupFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GroupFill: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


