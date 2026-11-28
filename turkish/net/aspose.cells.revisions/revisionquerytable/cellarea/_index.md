---
title: "RevisionQueryTable.CellArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionQueryTable özelliği. Etkilenen sorgu tablosunun konumunu alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

Etkilenen sorgu tablosunun konumunu alır.

```csharp
public CellArea CellArea { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // Gerçek bir senaryoda, revizyonları workbook'tan alırsınız
                // Demonstrasyon için, kavramsal bir örnek oluşturacağız
                // Not: RevisionQueryTable örnekleri genellikle çalışma kitabı revizyonlarından elde edilir
                RevisionQueryTable revisionQueryTable = null;

                // Bir revizyon sorgu tablosu olup olmadığını kontrol edin
                if (revisionQueryTable != null)
                {
                    // CellArea özelliği değerini göster (yalnızca okunabilir)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // Bağlam için diğer özellikleri göster
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("CellAreaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


