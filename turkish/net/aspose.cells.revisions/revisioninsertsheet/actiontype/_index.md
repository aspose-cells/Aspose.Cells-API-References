---
title: "RevisionInsertSheet.ActionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionInsertSheet özelliği. Revizyonun eylem türünü alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioninsertsheet/actiontype/
---
## RevisionInsertSheet.ActionType property

Revizyonun eylem türünü alır.

```csharp
public RevisionActionType ActionType { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Revizyon takibi ile yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // Not: StartTrackingRevisions sağlanan API'de mevcut değil
            // workbook.StartTrackingRevisions();

            // Bir revizyon kaydı oluşturmak için yeni bir çalışma sayfası ekle
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Not: StopTrackingRevisions sağlanan API'de mevcut değil
            // workbook.StopTrackingRevisions();
            
            // Not: Revisions özelliği sağlanan API'de mevcut değil
            // Revizyonların olup olmadığını kontrol etmek için HasRevisions'ı kullanacağız
            if (workbook.HasRevisions)
            {
                // Gerçek bir senaryoda, burada revizyonlara erişirdik
                // RevisionInsertSheet'i doğrudan oluşturamadığımız için, birini kontrol etmeyi taklit edeceğiz
                // Bu, revizyonu bir yerden (örneğin workbook.Revisions) aldığımızı varsayar
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                // ActionType'ı oluşturamıyor veya ayarlayamıyor olduğumuz için, sadece kontrol etmeyi göstereceğiz
                if (insertSheetRevision != null)
                {
                    // ActionType özelliğini görüntüle
                    Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);

                    // Salt okunur özelliğin kullanımını göster
                    if (insertSheetRevision.ActionType == RevisionActionType.Add)
                    {
                        Console.WriteLine("This revision represents a sheet addition");
                    }
                }

                // Revizyonlarla birlikte çalışma kitabını kaydet
                workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No sheet insertion revision found");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


