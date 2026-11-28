---
title: "XpsSaveOptions.XpsSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XpsSaveOptions yapıcı. XPS dosyası kaydetmek için seçenekler oluşturur"
type: docs
url: /tr/net/aspose.cells/xpssaveoptions/xpssaveoptions/
---
## XpsSaveOptions() {#constructor}

xps dosyasını kaydetmek için seçenekler oluşturur.

```csharp
public XpsSaveOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XpsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("XPS Save Options Demo");

            // Yapıcıyı kullanarak XpsSaveOptions başlat
            XpsSaveOptions saveOptions = new XpsSaveOptions();

            // Kaydetme seçeneklerini yapılandır
            saveOptions.OnePagePerSheet = true;
            saveOptions.DefaultFont = "Arial";
            saveOptions.PageIndex = 0;
            saveOptions.PageCount = 1;

            // Seçeneklerle çalışma kitabını kaydet
            workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XpsSaveOptions(SaveFormat) {#constructor_1}

xps dosyasını kaydetmek için seçenekler oluşturur.

```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | SaveFormat | Kaydetme formatı, xps formatı olmalıdır. |

### Açıklamalar

NOT: Bu yapıcı artık kullanımdan kaldırılmıştır. Bunun yerine lütfen XpsSaveOptions() yapıcısını kullanın. Bu özellik, Ağustos 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XpsSaveOptionsMethodSharpctorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "XPS Save Options Demo";
            worksheet.Cells["B1"].Value = "Using SaveFormat parameter";

            try
            {
                // SaveFormat parametresiyle yapıcıyı kullanarak XpsSaveOptions oluşturun
                XpsSaveOptions saveOptions = new XpsSaveOptions(SaveFormat.Xps);

                // Çalışma kitabını belirtilen seçeneklerle kaydedin
                workbook.Save("XpsSaveOptionsWithSaveFormatDemo.xps", saveOptions);

                Console.WriteLine("XpsSaveOptions created successfully with SaveFormat parameter");
                Console.WriteLine("Workbook saved as XPS format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating XpsSaveOptions or saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


