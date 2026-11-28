---
title: "TxtLoadOptions.TxtLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions yapıcı. Metin dosyasını yüklemek için seçenekleri oluşturur"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/txtloadoptions/
---
## TxtLoadOptions() {#constructor}

Metin dosyası yükleme seçeneklerini oluşturur.

```csharp
public TxtLoadOptions()
```

### Açıklamalar

Varsayılan yükleme dosya türü CSV'dir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yapıcıyı kullanarak yeni TxtLoadOptions oluşturun
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            
            // CSV dosyası için ayırıcıyı ayarlayın
            loadOptions.Separator = ',';
            
            // Yükleme seçenekleriyle bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Yüklenen dosyadan bazı bilgileri çıktı olarak verin
            Console.WriteLine("Worksheet count: " + workbook.Worksheets.Count);
            Console.WriteLine("First cell value: " + workbook.Worksheets[0].Cells["A1"].Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtLoadOptions(LoadFormat) {#constructor_1}

Metin dosyası yükleme seçeneklerini oluşturur.

```csharp
public TxtLoadOptions(LoadFormat loadFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadFormat | LoadFormat | Yükleme biçimi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class TxtLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Örnek CSV içeriği ve geçici dosya oluşturun
            string csvData = "Column1,Column2,Column3\nData1,Data2,Data3";
            string tempFile = Path.GetTempFileName();
            File.WriteAllText(tempFile, csvData);

            try
            {
                // LoadFormat.Csv ile TxtLoadOptions oluşturun
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
                loadOptions.Separator = ',';
                loadOptions.HasTextQualifier = true;

                // Yapılandırılmış seçenekleri kullanarak CSV'yi yükleyin
                Workbook workbook = new Workbook(tempFile, loadOptions);
                Worksheet worksheet = workbook.Worksheets[0];

                // Yüklenen verileri gösterin
                Console.WriteLine($"A1 Cell Value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 Cell Value: {worksheet.Cells["B2"].StringValue}");

                // İşlenmiş çalışma kitabını kaydet
                workbook.Save("TxtLoadOptionsCtorDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing constructor: {ex.Message}");
            }
            finally
            {
                // Geçici dosyayı temizle
                if (File.Exists(tempFile))
                {
                    File.Delete(tempFile);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


