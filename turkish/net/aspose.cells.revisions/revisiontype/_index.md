---
title: "RevisionType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionType enum. Revizyon türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Revizyon tipini temsil eder.

```csharp
public enum RevisionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| CustomView | `0` | Özel görünüm. |
| DefinedName | `1` | Tanımlı ad. |
| ChangeCells | `2` | Hücre değişikliği. |
| AutoFormat | `3` | Otomatik biçim. |
| MergeConflict | `4` | Birleştirme çakışması. |
| Comment | `5` | Yorum. |
| Format | `6` | Biçim. |
| InsertSheet | `7` | Çalışma sayfası ekle. |
| MoveCells | `8` | Hücreleri taşı. |
| Undo | `9` | Geri al. |
| QueryTable | `10` | Tabloyu sorgula. |
| InsertDelete | `11` | Ekleme veya silme. |
| RenameSheet | `12` | Çalışma sayfasını yeniden adlandır. |
| Unknown | `13` | Bilinmiyor. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Farklı RevisionType enum değerlerini kullanmayı gösterin
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // Enum değerlerini ve bunların temel tamsayı değerlerini göster
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // Revizyon türlerini kontrol etmeyi gösterin
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


