---
title: "LoadOptions.LoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions yapıcı. Dosyanın yüklenmesi için bir seçenek oluşturur"
type: docs
url: /tr/net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Dosyayı yükleme seçeneklerini oluşturur.

```csharp
public LoadOptions()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";

            try
            {
                // Örnek CSV içeriği oluşturun
                File.WriteAllText(tempCsvPath, "Name,Age\nJohn,30\nJane,25");

                // Varsayılan yapıcıyı göster
                LoadOptions defaultOptions = new LoadOptions();
                Console.WriteLine("Default LoadFormat: " + defaultOptions.LoadFormat);

                // LoadFormat parametresiyle yapıcıyı göster
                LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
                Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

                // Belirtilen seçeneklerle CSV dosyasını yükle
                Workbook workbook = new Workbook(tempCsvPath, csvOptions);

                // Verilerin doğru yüklendiğini doğrula
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"Cell A1: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"Cell B2: {worksheet.Cells["B2"].StringValue}");

                // Dönüşümü göstermek için XLSX olarak kaydet
                workbook.Save("CsvToExcel.xlsx");
                Console.WriteLine("CSV file successfully loaded and converted to XLSX");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Dosyayı yükleme seçeneklerini oluşturur.

```csharp
public LoadOptions(LoadFormat loadFormat)
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
    using System.IO;

    public class LoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            string tempCsvPath = "temp_input.csv";
            
            try
            {
                // Örnek CSV içeriği oluşturun
                File.WriteAllText(tempCsvPath, "Column1,Column2\nData1,Data2");

                // LoadFormat.Csv ile LoadOptions oluştur
                LoadOptions options = new LoadOptions(LoadFormat.Csv);

                // Oluşturulan seçeneklerle CSV dosyasını yükle
                Workbook workbook = new Workbook(tempCsvPath, options);

                // Hücreyi okuyarak başarılı yüklemeyi göster
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine($"A1 cell value: {worksheet.Cells["A1"].StringValue}");
                Console.WriteLine($"B2 cell value: {worksheet.Cells["B2"].StringValue}");

                // Dönüşüm yeteneğini göstermek için XLSX olarak kaydet
                workbook.Save("CsvLoadedAsExcel.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during CSV loading: {ex.Message}");
            }
            finally
            {
                if (File.Exists(tempCsvPath))
                    File.Delete(tempCsvPath);
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


