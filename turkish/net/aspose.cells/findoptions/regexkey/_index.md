---
title: "FindOptions.RegexKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FindOptions özelliği. Aranan anahtarın regex olup olmadığını gösterir. True ise aranan anahtar regex olarak alınır ve ayrıştırılır. Aksi takdirde anahtar, MS Excel'deki kurallara göre ayrıştırılır."
type: docs
url: /tr/net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

Aranan anahtarın regex olup olmadığını gösterir. Doğru ise aranan anahtar regex olarak alınır ve ayrıştırılır. Aksi takdirde anahtar MS Excel'deki kurallara göre ayrıştırılır.

```csharp
public bool RegexKey { get; set; }
```

### Açıklamalar

Arama anahtarı regex olarak belirtilmiş olsa da, belirtilen [`LookAtType`](../lookattype/) göre yeniden düzenlenebilir. Örneğin, tür Contains olduğunda (bu seçeneklerin varsayılan değeri), arama anahtarının başına ve sonuna otomatik olarak joker karakterler eklenir, böylece eşleşme "contains" olarak kontrol edilir. Bu durumda, düzenli ifadeler daha karmaşık hâle gelir ve performans da düşer. Bu nedenle, performans açısından, kullanıcı regex için kesin kuralı belirtmişse, ek bir kısıtlama olarak [`LookAtType`](../lookattype/) kullanmaya gerek yoktur ve kullanıcı daha iyi performans elde etmek için EntireContent olarak ayarlayabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Desen eşleşen dizelerle test verisi ayarlayın
            worksheet.Cells["A1"].PutValue("[hello]");
            worksheet.Cells["A2"].PutValue("Regular text");
            worksheet.Cells["A3"].PutValue("[another_example]");

            // Regex etkinleştirilmiş bulma seçenekleri oluşturun
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;

            // Regex desenine uyan hücreleri arayın
            string regEx = "\\[[a-zA-Z0-9_]+\\]";
            Cell foundCell = worksheet.Cells.Find(regEx, null, options);

            // Sonucu çıktı olarak ver
            if (foundCell != null)
            {
                Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
            }
            else
            {
                Console.WriteLine("No matching cells found");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


