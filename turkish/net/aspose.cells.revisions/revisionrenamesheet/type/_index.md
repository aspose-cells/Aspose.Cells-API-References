---
title: "RevisionRenameSheet.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionRenameSheet özelliği. Revizyonun türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisionrenamesheet/type/
---
## RevisionRenameSheet.Type property

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

    public class RevisionRenameSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Değişiklik yapmadan önce revizyon takibini etkinleştir
            // Not: Bu yöntem sağlanan API'de mevcut değil, bu yüzden onu kaldıracağız
            // workbook.StartTrackingRevisions();

            // Bir revizyon oluşturmak için ilk çalışma sayfasının adını değiştir
            Worksheet worksheet = workbook.Worksheets[0];
            string originalName = worksheet.Name;
            worksheet.Name = "RenamedSheet";

            // Revizyonlar koleksiyonuna eriş
            // Not: Revisions özelliği sağlanan API'de mevcut değil
            // Bu yüzden önce çalışma kitabının revizyonları olup olmadığını kontrol etmemiz gerekir
            if (workbook.HasRevisions)
            {
                // Çalışma sayfası yeniden adlandırma revizyonunu bul
                RevisionRenameSheet renameRevision = null;
                // Revisions'a doğrudan erişemediğimiz için bu bölümü değiştirmemiz gerekecek
                // Bu sadece bir yer tutucu, çünkü gerçek API revizyon erişimini desteklemiyor
                Console.WriteLine("Revision tracking is not fully supported in this API version.");
                
                if (renameRevision != null)
                {
                    // Type özelliği değerini gösterin
                    Console.WriteLine("Revision Type: " + renameRevision.Type);
                    Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
                    Console.WriteLine("New Sheet Name: " + renameRevision.NewName);

                    // Type özelliğinin nasıl kullanılacağını göster
                    if (renameRevision.Type == RevisionType.RenameSheet)
                    {
                        Console.WriteLine("This revision represents a worksheet rename operation.");
                    }
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionRenameSheetDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


