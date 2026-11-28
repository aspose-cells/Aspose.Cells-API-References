---
title: "Cell.HasCustomStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrenin, ilgili satır, sütun veya çalışma kitabından devralınan varsayılan stilden farklı özelleştirilmiş stil ayarlarına sahip olup olmadığını gösterir."
type: docs
url: /tr/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

Bu hücrenin, ilgili satır, sütun veya çalışma kitabından devralınan varsayılan stilden farklı özel stil ayarlarına sahip olup olmadığını gösterir.

```csharp
public bool HasCustomStyle { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // İlk HasCustomState değerini göster (varsayılan stili devralır)
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // Özel bir stil oluşturun ve hücreye uygulayın
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // Stil değişikliğinden sonra HasCustomStyle'ın true olduğunu doğrulayın
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // Özel stil uygulanmış çalışma kitabını kaydedin
            workbook.Save("CellCustomStyleDemo.xlsx");

            // Hücrenin stilini çalışma kitabının varsayılan stiline sıfırlayın
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // Varsayılan stile geri döndükten sonra HasCustomStyle'ın false olduğunu doğrulayın
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


