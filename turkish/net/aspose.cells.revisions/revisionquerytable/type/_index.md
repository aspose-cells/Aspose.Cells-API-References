---
title: "RevisionQueryTable.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionQueryTable özelliği. Revizyonun tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

Revizyonun türünü temsil eder.

```csharp
public override RevisionType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyTypeDemo
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

                // Sahte bir RevisionQueryTable oluşturun (bu kavramsaldır - gerçekte revizyonlardan alırsınız)
                // RevisionQueryTable'ı doğrudan örnekleyemediğimiz için, deseni göstereceğiz
                RevisionQueryTable revisionQueryTable = null;

                // Bir revizyon sorgu tablosu olup olmadığını kontrol edin
                if (revisionQueryTable != null)
                {
                    // Type özelliği değerini göster (yalnızca okunabilir)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // Referans için enum değerini tamsayı olarak göster
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // Bağlam için diğer özellikleri göster
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // Çalışma kitabını kaydedin
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


