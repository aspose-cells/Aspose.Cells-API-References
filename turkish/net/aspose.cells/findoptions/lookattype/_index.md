---
title: "FindOptions.LookAtType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Bakış tipi"
type: docs
url: /tr/net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

Türüne bak.

```csharp
public LookAtType LookAtType { get; set; }
```

### Açıklamalar

When [`RegexKey`](../regexkey/) doğru olduğunda ve kullanıcı regex için kesin kuralı belirttiğinde, performans açısından bu özellik EntireContent olarak ayarlanmalıdır. Aksi takdirde, arama anahtarını belirli türe göre eşleşebileceği şekilde yeniden düzenleyeceğiz. Örneğin, tür Contains olduğunda (bu özellik için varsayılan değerdir), arama anahtarının başına ve sonuna otomatik olarak joker karakterler ekleyeceğiz. Bu durumda, düzenli ifadeler daha karmaşık hâle gelecek ve performans da azalacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookAtTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun ve bazı veriler ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("=1+2"); // Formula
            worksheet.Cells["A3"].PutValue("Partial match test");
            worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells

            // LookAtType.EntireContent ile FindOptions oluştur
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.EntireContent
            };

            // Tam olarak "=A1&A3" ile eşleşen formülü ara
            Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
            Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));

            // Kısmi eşleşmeye değiştir
            options.LookAtType = LookAtType.Contains;
            cell = worksheet.Cells.Find("A3", null, options);
            Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
        }
    }
}
```

### Ayrıca Bakınız

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


