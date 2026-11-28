---
title: "Sınıf RevisionCustomView"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionCustomView sınıfı. Çalışma kitabına özel bir görünüm ekleme veya kaldırma işlemine ilişkin bir revizyon kaydını temsil eder."
type: docs
url: /tr/net/aspose.cells.revisions/revisioncustomview/
---
## RevisionCustomView class

Çalışma kitabına özel bir görünüm ekleme veya kaldırma için bir revizyon kaydını temsil eder.

```csharp
public class RevisionCustomView : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncustomview/actiontype/) { get; } | İşlemin türünü alır. |
| [Guid](../../aspose.cells.revisions/revisioncustomview/guid/) { get; } | Özel görünümün küresel olarak benzersiz tanımlayıcısını alır. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisioncustomview/type/) { get; } | Revizyon tipini alır. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCustomViewDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Bir revizyon oluşturmak için özel bir görünüm ekleyin
                // Not: CustomViews mevcut olmadığından geçici çözüm olarak CustomDocumentProperties kullanılıyor
                workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");

                // Revizyon günlüklerine erişin (var oldukları varsayılırsa)
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Yalnızca okunabilir özellikleri gösterin
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Action Type: {customViewRevision.ActionType}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");

                            // Özelliklerin temel kullanımını gösterin
                            if (customViewRevision.Type == RevisionType.CustomView)
                            {
                                Console.WriteLine("This is a custom view revision.");
                            }

                            if (customViewRevision.ActionType == RevisionActionType.Add)
                            {
                                Console.WriteLine("The custom view was added.");
                            }
                            else if (customViewRevision.ActionType == RevisionActionType.Delete)
                            {
                                Console.WriteLine("The custom view was deleted.");
                            }
                        }
                    }
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionCustomViewDemo.xlsx");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


