---
title: "RevisionCustomView.ActionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCustomView özelliği. Eylem türünü alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

İşlemin türünü alır.

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

    public class RevisionCustomViewPropertyActionTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Özel görünüm revizyonları içerebilecek mevcut bir çalışma kitabını yükle
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // Çalışma kitabındaki tüm revizyon günlükleri üzerinde yinele
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // Günlükteki her revizyonu kontrol et
                    foreach (Revision revision in log.Revisions)
                    {
                        // Bunun özel bir görünüm revizyonu olup olmadığını kontrol et
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // ActionType özelliği değerini göster
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // ActionType özelliğinin nasıl kullanılacağını göster
                            switch (customViewRevision.ActionType)
                            {
                                case RevisionActionType.Add:
                                    Console.WriteLine("This revision represents adding a custom view");
                                    break;
                                case RevisionActionType.Delete:
                                    Console.WriteLine("This revision represents deleting a custom view");
                                    break;
                                default:
                                    Console.WriteLine("This revision represents another type of action");
                                    break;
                            }

                            // Bağlam için ek özellikleri göster
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");
                        }
                    }
                }
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

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


