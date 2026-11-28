---
title: "Name.Comment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name özelliği. İsmin yorumunu alır ve ayarlar. Yalnızca Excel 2007 veya daha yüksek sürümler için geçerlidir."
type: docs
url: /tr/net/aspose.cells/name/comment/
---
## Name.Comment property

Adın yorumunu alır ve ayarlar. Yalnızca Excel 2007 veya daha yeni sürümler için geçerlidir.

```csharp
public string Comment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyCommentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yorumlu bir adlandırılmış aralık ekle
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            namedRange.Comment = "This is a test named range";
            
            // Çalışma kitabını kaydedin
            workbook.Save("NamedRangeWithComment.xlsx");
            
            // Yorumu doğrulamak için kaydedilmiş çalışma kitabını yükle
            Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
            Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
            
            // İşlevselliği göstermek için yorumu çıktı olarak ver
            Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


