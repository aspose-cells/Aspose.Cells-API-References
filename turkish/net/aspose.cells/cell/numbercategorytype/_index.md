---
title: "Cell.NumberCategoryType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrenin sayı biçimlendirme kategorisini temsil eder"
type: docs
url: /tr/net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Bu hücrenin sayı biçimlendirmesinin kategori türünü temsil eder.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Açıklamalar

Hücrenin biçimlendirme deseni koşullu biçimlendirme desenleriyle birleştirildiğinde, döndürülen tür, bu hücrenin mevcut değeri için kullanılan bölüme karşılık gelir. Örneğin, bu hücre için biçimlendirme deseni "#,##0;(#,##0);"-";@" ise, hücrenin değeri sayısal ve 0 değilse döndürülen tür Number; hücrenin değeri 0 veya sayısal değilse döndürülen tür Text olur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNumberCategoryTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine bir tarih değeri ekleyin
            Cell dateCell = worksheet.Cells["A1"];
            dateCell.PutValue(DateTime.Now);
            
            // Tarih biçimini ayarlayın
            Style dateStyle = dateCell.GetStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            dateCell.SetStyle(dateStyle);
            
            // A2 hücresine sayısal bir değer ekleyin
            Cell numberCell = worksheet.Cells["A2"];
            numberCell.PutValue(1234.56);
            
            // A3 hücresine metin değeri ekleyin
            Cell textCell = worksheet.Cells["A3"];
            textCell.PutValue("Sample Text");
            
            // Her hücre için NumberCategoryType'ı gösterin
            Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
            Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
            Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
            
            // A2'yi para birimi biçimine değiştirin ve NumberCategoryType'ı kontrol edin
            Style currencyStyle = numberCell.GetStyle();
            currencyStyle.Custom = "$#,##0.00";
            numberCell.SetStyle(currencyStyle);
            Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


