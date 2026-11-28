---
title: "Worksheet.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Başka bir çalışma sayfasından içerik ve biçimleri kopyalar"
type: docs
url: /tr/net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Başka bir çalışma sayfasından içerik ve biçimleri kopyalar.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceSheet | Çalışma Sayfası | Kaynak çalışma sayfası. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir kaynak çalışma kitabı oluştur
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Worksheet");
            
            // Bir hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Kaynak çalışma sayfasını hedef çalışma sayfasına kopyala
            destSheet.Copy(sourceSheet);
            
            // Sonucu kaydet
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Başka bir çalışma sayfasından içerik ve biçimleri kopyalar.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceSheet | Çalışma Sayfası | Kaynak çalışma sayfası. |
| copyOptions | CopyOptions |  |

### Açıklamalar

Aynı dosyadaki veya başka bir dosyadaki başka bir çalışma sayfasından veri kopyalayabilirsiniz. Ancak, bu yöntem yorumlar, resimler ve grafikler gibi çizim nesnelerini kopyalamayı desteklemez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren kaynak çalışma kitabını oluşturun
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Name = "SourceSheet";
            srcSheet.Cells["A1"].PutValue("Source Data");

            // Hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            destSheet.Name = "DestinationSheet";

            // Kopyalama seçeneklerini yapılandır
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            // Seçeneklerle çalışma sayfasını kopyala
            srcSheet.Copy(destSheet, options);

            // Kopyalama işlemini doğrula
            Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
            
            // Sonucu kaydet
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


