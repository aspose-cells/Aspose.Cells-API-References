---
title: "Enum ParameterType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ParameterType enum. Fonksiyonun tüm parametre tiplerini veya dönüş değeri tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/parametertype/
---
## ParameterType enumeration

Fonksiyonun tüm parametre tiplerini veya dönüş değeri tipini temsil eder.

```csharp
public enum ParameterType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ParameterTypeDemo
    {
        public static void ParameterTypeExample()
        {
            // Kullanımı göstermek için bir çalışma kitabı ve çalışma sayfası oluşturma
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Formül işlevinde ParameterType enum'unun örnek kullanımı
            // Belirli parametre tipleriyle özel bir işlev tanımladığımızı varsayalım

            // Parametre tiplerinin bir dizisini tanımla
            ParameterType[] parameterTypes = new ParameterType[]
            {
                ParameterType.Reference,
                ParameterType.Value,
                ParameterType.Array
            };

            // Bu parametre tiplerini kullanan örnek işlev
            // Örneğin, tanımlı parametre tiplerine sahip varsayımsal bir özel işlev ayarlamak
            // (Not: Özel işlev işleme, Aspose.Cells API yeteneklerine bağlı olacaktır)

            // Değişiklikleri göstermek için çalışma kitabını kaydet
            workbook.Save("ParameterTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


