---
title: "FindOptions sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FindOptions sınıfı. Bulma seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/findoptions/
---
## FindOptions class

Bulma seçeneklerini temsil eder.

```csharp
public class FindOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FindOptions](findoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Aranan dizge değerini sayısal veriye dönüştürüp dönüştürmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Aranan aralığın ayarlanıp ayarlanmadığını gösterir. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Türüne bak. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Tür içinde bak. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Aranan anahtarın regex olup olmadığını gösterir. Doğru ise aranan anahtar regex olarak alınır ve ayrıştırılır. Aksi takdirde anahtar MS Excel'deki kurallara göre ayrıştırılır. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Hücreler için geriye doğru arama yapılıp yapılmayacağını belirtir. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) Arama sırası. True: bir sonraki aranır. False: önceki aranır. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Arama sırasının satır mı yoksa sütun mu olduğunu gösterir. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | Aranacak format. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Aranan hücre değer tipinin aranan anahtar ile aynı olması gerekip gerekmediğini gösterir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Aranan aralığı alır ve ayarlar. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Aranan aralığı ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsDemo
    {
        public static void FindOptionsExample()
        {
            // Çalışma kitabı nesnesini örnekle
            Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");

            // Hücreler koleksiyonunu al
            Cells cells = workbook.Worksheets[0].Cells;

            // FindOptions nesnesini örnekle
            FindOptions findOptions = new FindOptions();

            // Bir Hücre Alanı oluştur
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // FindOptions için hücre alanını ayarla
            findOptions.SetRange(ca);

            // Arama özelliklerini ayarla
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // 0 değerine sahip hücreyi bul
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine("Cell found at: " + cell.Name);
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


