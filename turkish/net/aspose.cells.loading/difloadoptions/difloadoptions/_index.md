---
title: "DifLoadOptions.DifLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DifLoadOptions yapıcı. Seçenekler"
type: docs
url: /tr/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

Seçenekler.

```csharp
public DifLoadOptions()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Parametresiz yapıcıyı kullanarak DifLoadOptions'ın yeni bir örneğini oluşturun
                DifLoadOptions loadOptions = new DifLoadOptions();

                // Varsayılan seçeneklerle yeni bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook();

                // İlk çalışma sayfasına eriş
                Worksheet worksheet = workbook.Worksheets[0];

                // Çalışma kitabının işlevsel olduğunu göstermek için örnek veri ekleyin
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // Çalışma kitabını DIF formatında kaydedin
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // Şimdi kaydedilmiş DIF dosyasını DifLoadOptions ile yükleyin
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // Yüklenen verileri doğrulama için XLSX olarak kaydedin
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


