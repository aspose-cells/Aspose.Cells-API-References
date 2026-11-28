---
title: "HtmlLoadOptions.HtmlLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions yapıcı. Dosyanın yüklenmesi için bir seçenek oluşturur"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/htmlloadoptions/
---
## HtmlLoadOptions() {#constructor}

Dosyayı yükleme seçeneklerini oluşturur.

```csharp
public HtmlLoadOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yapıcıyı kullanarak HTML yükleme seçenekleri oluşturun
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;

            // Seçeneklerle HTML dosyasını yükleyin
            Workbook workbook = new Workbook("example.html", loadOptions);

            // Yüklenen HTML'den verilere erişin
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("B1 Cell Value: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("B3 Cell Value: " + worksheet.Cells["B3"].StringValue);
            Console.WriteLine("B4 Cell Value: " + worksheet.Cells["B4"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlLoadOptions(LoadFormat) {#constructor_1}

Dosyayı yükleme seçeneklerini oluşturur.

```csharp
public HtmlLoadOptions(LoadFormat loadFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadFormat | LoadFormat | Yükleme formatı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            try
            {
                // LoadFormat parametresiyle yapıcıyı kullanarak HtmlLoadOptions örneği oluşturun
                HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);

                // HtmlLoadOptions'ın bazı özelliklerini ayarlayın
                loadOptions.AutoFitColsAndRows = true;
                loadOptions.SupportDivTag = true;
                loadOptions.DeleteRedundantSpaces = true;

                // Yükleme seçeneklerini kullanarak bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook("input.html", loadOptions);

                // İlk çalışma sayfasına eriş
                Worksheet worksheet = workbook.Worksheets[0];

                // Yüklenen HTML hakkında bazı bilgileri görüntüle
                Console.WriteLine("HTML loaded successfully with LoadFormat.Html");
                Console.WriteLine($"Worksheet name: {worksheet.Name}");
                Console.WriteLine($"Cells count: {worksheet.Cells.MaxDataRow + 1} rows x {worksheet.Cells.MaxDataColumn + 1} columns");

                // Çalışma kitabını kaydedin
                workbook.Save("HtmlLoadOptionsCtorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading HTML file: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


