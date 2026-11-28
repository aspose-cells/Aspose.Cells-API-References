---
title: "ImportTableOptions.DefaultValues"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Tablodaki değerin varsayılan değeri null'dır"
type: docs
url: /tr/net/aspose.cells/importtableoptions/defaultvalues/
---
## ImportTableOptions.DefaultValues property

Tablodaki değer için varsayılan değer null'dur.

```csharp
public object[] DefaultValues { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyDefaultValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Null değerli örnek veri oluştur
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Quantity", typeof(int));
            dataTable.Columns.Add("ExpiryDate", typeof(DateTime));
            
            dataTable.Rows.Add("Bread", 10, DateTime.Now.AddDays(7));
            dataTable.Rows.Add(null, null, null); // Will use default values
            dataTable.Rows.Add("Milk", null, DateTime.Now.AddDays(3));

            ImportTableOptions importOptions = new ImportTableOptions();
            
            // İlk durumu göster
            Console.WriteLine("Current DefaultValues: " + (importOptions.DefaultValues == null ? "Not set" : "Set"));

            // Her sütun için varsayılan değerleri yapılandır
            importOptions.DefaultValues = new object[] { "[Unspecified]", 1, DateTime.Today };

            // Boş değer işleme ile verileri içe aktar
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Daha iyi görünürlük için sütunları otomatik sığdır
            worksheet.AutoFitColumns();

            workbook.Save("DefaultValuesDemo.xlsx");
            Console.WriteLine("Spreadsheet saved with default values applied to null entries.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


