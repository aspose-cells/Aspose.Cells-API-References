---
title: "PivotPageFields.PageFieldCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotPageFields özelliği. Sayfa alanlarının sayısını alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

Sayfa alanlarının sayısını alır.

```csharp
public int PageFieldCount { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Veri içeren örnek çalışma sayfaları oluştur
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Data1";
            FillSampleData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Data2");
            FillSampleData(sheet2);

            // Bir pivot sayfası oluştur
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");

            // PivotPageFields örneği oluştur
            PivotPageFields pageFields = new PivotPageFields();

            // PageFieldCount özelliğini göstermek için sayfa alanları ekle
            pageFields.AddPageField(new string[] { "Category1", "Category2" });
            pageFields.AddPageField(new string[] { "Region1", "Region2" });

            try
            {
                // PageFieldCount özelliği değerini göster
                Console.WriteLine("Number of page fields: " + pageFields.PageFieldCount);

                // Sayfa alanları için tanımlama ekleyin
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                pageFields.AddIdentify(1, new int[] { 1, 0 });

                // Tanımlamalar eklendikten sonra sayının aynı kalıp kalmadığını doğrulayın
                Console.WriteLine("PageFieldCount after adding identifications: " + pageFields.PageFieldCount);

                // Sayfa alanlarını kullanarak pivot tablo oluşturun
                string[] sources = { "=Data1!A1:C4", "=Data2!A1:C4" };
                pivotSheet.PivotTables.Add(sources, false, pageFields, "E3", "DemoPivot");

                // Çalışma kitabını kaydedin
                workbook.Save("PageFieldCountDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static void FillSampleData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Value");

            cells["A2"].PutValue("Category1");
            cells["B2"].PutValue("Region1");
            cells["C2"].PutValue(100);

            cells["A3"].PutValue("Category2");
            cells["B3"].PutValue("Region2");
            cells["C3"].PutValue(200);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


