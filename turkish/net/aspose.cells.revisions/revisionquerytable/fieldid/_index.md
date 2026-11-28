---
title: "RevisionQueryTable.FieldId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionQueryTable özelliği. Kaldırılan belirli sorgu tablosu alanının kimliğini alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Kaldırılan belirli sorgu tablosu alanının kimliğini alır.

```csharp
public int FieldId { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
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
                // Bir sorgu tablosu oluşturun (bu basitleştirilmiş bir örnektir)
                // Not: Gerçek bir senaryoda, önce bir sorgu tablosu oluşturmanız gerekir
                // Demonstrasyon amacıyla, bir RevisionQueryTable erişimini taklit edeceğiz

                // Bu basitleştirilmiş örnekte doğrudan bir RevisionQueryTable oluşturamadığımız için,
                // eğer bir FieldId özelliğimiz olsaydı, ona nasıl erişileceğini göstereceğiz
                // Bu, yalnızca okunabilir özelliği okuma desenini gösterir

                // Revizyonlardan bir RevisionQueryTable almayı taklit edin (kavramsal)
                // Gerçekte, bunu workbook.Revisions veya benzerinden alırsınız
                RevisionQueryTable revisionQueryTable = null;

                // Bir revizyon sorgu tablosu olup olmadığını kontrol edin (bu sadece gösterim içindir)
                if (revisionQueryTable != null)
                {
                    // FieldId özelliği değerini göster
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // Bağlam için diğer özellikleri göster
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("FieldIdDemo.xlsx");
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

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


