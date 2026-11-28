---
title: "Style.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. İki Style örneğinin eşit olup olmadığını belirler"
type: docs
url: /tr/net/aspose.cells/style/equals/
---
## Style.Equals method

İki Style örneğinin eşit olup olmadığını belirler.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Mevcut Style nesnesiyle karşılaştırılacak Style nesnesi. |

### Dönüş Değeri

Belirtilen Nesne mevcut Nesneye eşitse true; aksi takdirde false.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karşılaştırmak için iki stil oluştur
            Style style1 = workbook.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Arial";
            style2.Font.Size = 12;
            style2.HorizontalAlignment = TextAlignmentType.Center;

            try
            {
                // Stilleri karşılaştırmak için Equals yöntemini çağır
                bool areEqual = style1.Equals((object)style2);

                // Sonucu göster
                Console.WriteLine($"The styles are equal: {areEqual}");

                // Stilleri uygulayarak aynı olduklarını göster
                if (areEqual)
                {
                    Cell cell1 = worksheet.Cells["A1"];
                    cell1.PutValue("Style 1");
                    cell1.SetStyle(style1);

                    Cell cell2 = worksheet.Cells["A2"];
                    cell2.PutValue("Style 2");
                    cell2.SetStyle(style2);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("StyleEqualsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


