---
title: "DbfLoadOptions.DbfLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DbfLoadOptions yapıcı. Seçenekler"
type: docs
url: /tr/net/aspose.cells.loading/dbfloadoptions/dbfloadoptions/
---
## DbfLoadOptions constructor

Seçenekler.

```csharp
public DbfLoadOptions()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DbfLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // DbfLoadOptions örneğini #ctor yöntemiyle oluştur
                DbfLoadOptions loadOptions = new DbfLoadOptions();

                // DBF yükleme seçenekleriyle çalışma kitabı oluşturun
                Workbook workbook = new Workbook("sample.dbf", loadOptions);

                // İlk çalışma sayfasına eriş
                Worksheet worksheet = workbook.Worksheets[0];

                // Yüklenen DBF dosyasından bazı verileri göster
                Console.WriteLine("Data loaded from DBF file:");
                Console.WriteLine(worksheet.Cells["A1"].StringValue);

                // Çalışma kitabını Excel formatında kaydedin
                workbook.Save("DbfLoadOptionsCtorDemo.xlsx", SaveFormat.Xlsx);
                Console.WriteLine("File saved successfully with DBF data");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DbfLoadOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DbfLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


