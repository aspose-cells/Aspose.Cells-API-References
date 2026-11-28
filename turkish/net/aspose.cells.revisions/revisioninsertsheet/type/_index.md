---
title: "RevisionInsertSheet.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionInsertSheet özelliği. Revizyonun türünü alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioninsertsheet/type/
---
## RevisionInsertSheet.Type property

Revizyon tipini alır.

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

    public class RevisionInsertSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Revizyon takibi ile yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Revizyon takibini etkinleştir (StartTrackingRevisions mevcut olmadığından simüle edildi)
            bool trackRevisions = true;

            // Bir revizyon kaydı oluşturmak için yeni bir çalışma sayfası ekle
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Revizyonları almayı simüle et (Revisions özelliği mevcut olmadığından)
            if (trackRevisions && workbook.HasRevisions)
            {
                // Gerçek bir senaryoda, burada revizyonlara erişirdik
                // Bu, revizyonu bir yerden (örneğin workbook.Revisions) aldığımızı varsayar
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                if (insertSheetRevision != null)
                {
                    // Type özelliğini göster
                    Console.WriteLine("Revision Type: " + insertSheetRevision.Type);

                    // Yalnızca okunur Type özelliğinin kullanımını göster
                    if (insertSheetRevision.Type == RevisionType.InsertSheet)
                    {
                        Console.WriteLine("This revision represents a sheet insertion operation");
                        
                        // Eklenen sayfa hakkında ek bilgi göster
                        Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
                        Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
                    }

                    // Diğer revizyon türlerine karşı kontrol et
                    if (insertSheetRevision.Type != RevisionType.Unknown)
                    {
                        Console.WriteLine("This is a known revision type");
                    }
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No revisions found or revision tracking not enabled");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


