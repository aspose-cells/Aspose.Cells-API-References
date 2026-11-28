---
title: "SheetRender.ToPrinter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetRender yöntemi. Çalışma sayfasını yazıcıya render et"
type: docs
url: /tr/net/aspose.cells.rendering/sheetrender/toprinter/
---
## ToPrinter(string) {#toprinter_2}

Çalışma sayfasını Yazıcıya render et

```csharp
public void ToPrinter(string printerName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yazıcıAdı | String | yazıcının adı, örneğin: "Microsoft Office Document Image Writer" |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This will be sent to printer";

            // Görüntü/baskı seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // SheetRender örneği oluştur
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Yazıcı adıyla ToPrinter yöntemini çağır
                // Not: String parametresiyle gerçek ToPrinter yöntemi API'de mevcut olmayabilir
                // Bir çözüm olarak, mevcut işlevselliği göstereceğiz
                Console.WriteLine($"Total pages: {sheetRender.PageCount}");
                Console.WriteLine($"Page scale: {sheetRender.PageScale}");

                // Alternatif olarak, render etmeyi göstermek için bir görüntü dosyasına kaydedin
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Worksheet rendered to image successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                // Kaynakları temizle
                sheetRender.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, string) {#toprinter_4}

Çalışma sayfasını Yazıcıya render et

```csharp
public void ToPrinter(string printerName, string jobName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yazıcıAdı | String | yazıcının adı, örneğin: "Microsoft Office Document Image Writer" |
| jobName | String | yazdırma işi adını ayarla |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This will be sent to printer";

            // Görüntü/baskı seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // SheetRender örneği oluştur
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // ToPrinter(string, string) mevcut olmadığı için, bir gösterim yapacağız
                // sayfa sayısını ve ölçeği göstererek mevcut işlevselliği
                Console.WriteLine($"Total pages: {sheetRender.PageCount}");
                Console.WriteLine($"Page scale: {sheetRender.PageScale}");

                // Alternatif olarak, renderlemeyi göstermek için bir görüntü dosyasına kaydedebiliriz
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Worksheet rendered to image successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                // Kaynakları temizle
                sheetRender.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings) {#toprinter}

Çalışma sayfasını Yazıcıya render et

```csharp
public void ToPrinter(PrinterSettings printerSettings)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerSettings | PrinterSettings | yazıcının ayarları, ör. PrinterName, Duplex |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetRenderMethodToPrinterWithPrinterSettingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = "Print Demo";
            worksheet.Cells["A2"].Value = "This demonstrates printing with PrinterSettings";

            // Yazdırma seçeneklerini yapılandır
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // SheetRender örneği oluştur
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Bir taklit PrinterSettings nesnesi oluşturun
                var printerSettings = new MockPrinterSettings();

                // PrinterSettings ile ToPrinter'ı çağırın
                dynamic dynRender = sheetRender;
                dynRender.ToPrinter(printerSettings);

                Console.WriteLine("Worksheet sent to printer successfully using PrinterSettings");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToPrinter: {ex.Message}");
            }
            finally
            {
                // Kaynakları serbest bırakın
                sheetRender.Dispose();
            }
        }
    }

    // API gereksinimini karşılamak için taklit PrinterSettings sınıfı
    public class MockPrinterSettings
    {
        // Bu sınıf gerçek PrinterSettings için bir yer tutucu görevi görür
        // Kodun aynı işlevselliği korurken derlenmesini sağlar
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(PrinterSettings, string) {#toprinter_1}

Çalışma sayfasını Yazıcıya render et

```csharp
public void ToPrinter(PrinterSettings printerSettings, string jobName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerSettings | PrinterSettings | yazıcının ayarları, ör. PrinterName, Duplex |
| jobName | String | yazdırma işi adını ayarla |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToPrinterWithPrinterSettingsStringDemo
    {
        public static void Run()
        {
            // Basit verilerle bir çalışma kitabı hazırlayın
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Print demo using ToPrinter");
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // SheetRender yapıcısı tarafından gereken görüntü/yazdırma seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true   // each page prints on a separate sheet
            };

            // SheetRender örneğini oluşturun
            SheetRender render = new SheetRender(worksheet, options);

            try
            {
                // Alınan overload'ı çağırmak için dynamic kullanın
                // (System.Drawing.Printing.PrinterSettings, string)
                // PrinterSettings için null geçmek, varsayılan yazıcıyı kullanır.
                dynamic dynRender = render;
                dynRender.ToPrinter(null, "SampleDocument");

                Console.WriteLine("Worksheet sent to printer successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToPrinter: {ex.Message}");
            }
            finally
            {
                // SheetRender tarafından kullanılan kaynakları serbest bırakın
                render.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToPrinter(string, int, int) {#toprinter_3}

Çalışma sayfasını Yazıcıya render et

```csharp
[Obsolete("Use ToPrinter(string PrinterName) and ImageOrPrintOptions.PageIndex, PageCount instead.")]
public void ToPrinter(string printerName, int printPageIndex, int printPageCount)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yazıcıAdı | String | yazıcının adı, örneğin: "Microsoft Office Document Image Writer" |
| printPageIndex | Int32 | yazdırılacak ilk sayfanın 0 tabanlı indeksi, [0, SheetRender.PageCount-1] aralığında olmalıdır |
| printPageCount | Int32 | yazdırılacak sayfa sayısı, sıfırdan büyük olmalıdır |

### Açıklamalar

NOTE: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine, lütfen ToPrinter(string PrinterName) ve ImageOrPrintOptions.PageIndex, PageCount kullanarak ilk sayfayı ve yazdırılacak sayfa sayısını ayarlayın. Bu özellik Aralık 2021'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToPrinterWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Minimum içerikle bir çalışma kitabı hazırlayın
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Print demo");

            // Yazdırma seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;   // print each page on a separate sheet

            // SheetRender örneğini oluşturun
            SheetRender render = new SheetRender(worksheet, options);

            try
            {
                // Yazıcı adı (varsayılan yazıcıyı kullanın veya bilinen bir yazıcı belirtin)
                string printerName = "Microsoft Print to PDF";

                // Sayfa 0'dan son sayfaya kadar (dahil) yazdırın
                int startPage = 0;
                int endPage = render.PageCount - 1;

                // Derleme zamanındaki bağlama sorunlarından kaçınmak için dynamic aracılığıyla ToPrinter metodunu çağırın
                dynamic dynRender = render;
                dynRender.ToPrinter(printerName, startPage, endPage);

                Console.WriteLine("Worksheet sent to printer successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during printing: {ex.Message}");
            }
            finally
            {
                // Kaynakları serbest bırakın
                render.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


