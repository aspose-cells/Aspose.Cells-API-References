---
title: "Enum RevisionActionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionActionType enum. Revizyon eylemi türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisionactiontype/
---
## RevisionActionType enumeration

Revizyon eyleminin türünü temsil eder.

```csharp
public enum RevisionActionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Add | `0` | Revizyon ekle. |
| Delete | `1` | Revizyon sil. |
| DeleteColumn | `2` | Sütun silme revizyonu. |
| DeleteRow | `3` | Satır silme revizyonu. |
| InsertColumn | `4` | Sütun ekleme revizyonu. |
| InsertRow | `5` | Satır ekleme revizyonu. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionActionTypeDemo
    {
        public static void Run()
        {
            // Revizyon takibi ile yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı revizyon türleri oluşturan çeşitli işlemler gerçekleştir
            worksheet.Cells["A1"].PutValue("Initial Value");
            worksheet.Cells.InsertRow(0);
            worksheet.Cells.DeleteRow(1);
            worksheet.Cells.InsertColumn(0);
            worksheet.Cells.DeleteColumn(1);

            // Çalışma kitabının revizyonları olup olmadığını kontrol et
            if (workbook.HasRevisions)
            {
                // Not: Orijinal API, revizyon koleksiyonuna doğrudan erişim sağlamaz
                // Bu yüzden istenildiği gibi RevisionActionType enum'ını sadece göstereceğiz
                Console.WriteLine("Workbook contains revisions (but API doesn't provide access)");
            }

            // RevisionActionType enum değerlerini göster
            Console.WriteLine("Available revision action types:");
            foreach (RevisionActionType actionType in Enum.GetValues(typeof(RevisionActionType)))
            {
                Console.WriteLine($"{actionType} = {(int)actionType}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RevisionActionTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


