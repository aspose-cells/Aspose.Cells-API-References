---
title: "Enum LoadNumbersTableType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Numbers.LoadNumbersTableType enum. Bir sayfada bazı tablolar bulunduğunda tablo yükleme türünü belirtir"
type: docs
url: /tr/net/aspose.cells.numbers/loadnumberstabletype/
---
## LoadNumbersTableType enumeration

Bazı tablolar bir sayfada olduğunda tablo yükleme türünü gösterir.

```csharp
public enum LoadNumbersTableType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| OneTablePerSheet | `1` |  |
| OverrideOtherTables | `2` |  |
| TileTables | `4` |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Numbers;
    using System;

    public class LoadNumbersTableTypeDemo
    {
        public static void LoadNumbersTableTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Yeni bir çalışma sayfası oluştur
            Worksheet worksheet = workbook.Worksheets[0];

            // NumbersLoadOptions örneği oluştur
            NumbersLoadOptions loadOptions = new NumbersLoadOptions();

            // LoadNumbersTableType özelliğini ayarla
            loadOptions.LoadTableType = LoadNumbersTableType.OneTablePerSheet;

            // Belirtilen yükleme seçenekleriyle bir Numbers dosyası yükle
            workbook = new Workbook("LoadNumbersTableTypeExample_original.numbers", loadOptions);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("LoadNumbersTableTypeExample.xlsx");

            Console.WriteLine("Workbook loaded and saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Numbers](../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../)


