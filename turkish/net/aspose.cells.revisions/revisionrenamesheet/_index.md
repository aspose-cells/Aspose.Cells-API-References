---
title: "Sınıf RevisionRenameSheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionRenameSheet sınıfı. Sayfa yeniden adlandırmanın bir revizyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

Sayfa yeniden adlandırmanın bir revizyonunu temsil eder.

```csharp
public class RevisionRenameSheet : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | Çalışma sayfasının yeni adını alır. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | Çalışma sayfasının eski adını alır. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | Revizyonun türünü temsil eder. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Orijinal adı sakla ve sayfayı yeniden adlandır
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // Revizyonlar oluşturmak için bellek akışına kaydet
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // Revizyon günlüklerine erişmek için çalışma kitabını yeniden aç
                workbook = new Workbook(ms);

                // Yeniden adlandırma işlemi için revizyon günlüklerini kontrol et
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


