---
title: "RevisionInsertSheet.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionInsertSheet özelliği. Çalışma sayfasının adını alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Çalışma sayfasının adını alır.

```csharp
public string Name { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Potansiyel olarak bir revizyon kaydı oluşturmak için yeni bir çalışma sayfası ekleyin
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // Revizyonlardan bir RevisionInsertSheet'e erişimi simüle edin
                // Not: Gerçek bir senaryoda, bu workbook.Revisions'dan gelir
                // Demonstrasyon için, bir taklit senaryo oluşturacağız
                RevisionInsertSheet insertSheetRevision = null;

                // Gerçek kullanımda, bunu revizyonlar koleksiyonundan alırdınız
                // Örneğin: insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // RevisionInsertSheet'i doğrudan oluşturamadığımız için, göstereceğiz
                // birine erişiminiz olsaydı ne yapardınız
                if (insertSheetRevision != null)
                {
                    // Name özelliği değerini göster (yalnızca okunur)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // Koşullu bir kontrolde Name özelliğini kullanmayı göster
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


