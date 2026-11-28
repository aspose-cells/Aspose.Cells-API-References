---
title: "Sınıf RevisionDefinedName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionDefinedName sınıfı. Tanımlı ad değişikliğinin bir revizyon kaydını temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

Tanımlı ad değişikliği için bir revizyon kaydını temsil eder.

```csharp
public class RevisionDefinedName : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | Formülü alır. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | Eski formülü alır. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | Tanımlı adın metnini alır. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | Revizyonun türünü temsil eder. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Çalışma kitabına tanımlı bir ad ekle
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Bir revizyon oluşturmak için tanımlı adı değiştir
                definedName.RefersTo = "=Sheet1!$B$1";

                // Revizyon günlüklerini oluşturmak için çalışma kitabını kaydet
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // Revizyon bilgilerine erişmek için çalışma kitabını yeniden aç
                Workbook revisionWorkbook = new Workbook(filePath);

                // RevisionDefinedName girişlerini bulmak için revizyon günlüklerinde yineleme yap
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // RevisionDefinedName özelliklerini göster
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


