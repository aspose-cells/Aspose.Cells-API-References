---
title: "HorizontalPageBreakCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HorizontalPageBreakCollection özelliği. Belirtilen dizindeki HorizontalPageBreak öğesini alır"
type: docs
url: /tr/net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Belirtilen dizindeki [`HorizontalPageBreak`](../../horizontalpagebreak/) öğesini alır

```csharp
public HorizontalPageBreak this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yatay sayfa kesimleri ekleyin
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // Item özelliğini kullanarak sayfa sonlarına erişin
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // Sayfa sonlarını etkileyen hücreleri değiştirin
            worksheet.Cells.DeleteRows(0, 2);
            
            // Sayfa sonunun ayarlandığını doğrulayın
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Belirtilen hücre adıyla [`HorizontalPageBreak`](../../horizontalpagebreak/) öğesini alır.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| cellName | Hücre adı. |

### Dönüş Değeri

Belirtilen hücre adına sahip öğe.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class HorizontalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Farklı aşırı yüklemeler kullanarak birkaç yatay sayfa sonu ekleyin
                worksheet.HorizontalPageBreaks.Add(5);          // break after row index 5
                worksheet.HorizontalPageBreaks.Add("D5");      // break at cell D5 (row index 4)

                // ----- Tamsayı indeksiyle erişim (Item[int]) -----
                // Item özelliği indeksleyicidir, bu yüzden [] sözdizimini kullanırız
                HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
                Console.WriteLine("First break row (int index): " + firstBreak.Row);

                // ----- Dize anahtarıyla erişim (Item[string]) -----
                // D5 hücre adıyla eklenen sayfa sonunu alın
                HorizontalPageBreak breakByCell = worksheet.HorizontalPageBreaks["D5"];
                Console.WriteLine("Break added with \"D5\" is at row: " + breakByCell.Row);

                // Sayfa sonlarının kalıcı olduğunu doğrulamak için çalışma kitabını kaydedin
                workbook.Save("HorizontalPageBreaks_ItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


