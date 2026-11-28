---
title: "RevisionInsertDelete.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionInsertDelete özelliği. Revizyonun tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisioninsertdelete/type/
---
## RevisionInsertDelete.Type property

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

    public class RevisionInsertDeletePropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir workbook oluşturun ve revizyon izlemeyi etkinleştirin
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30; // Enable revision tracking by setting days

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir satır ekleyerek revizyon kaydı oluşturun
            worksheet.Cells.InsertRows(0, 1);

            // Revizyon koleksiyonunu alın (RevisionLogCollection kendisi koleksiyondur)
            RevisionLogCollection revisions = workbook.Worksheets.RevisionLogs;

            // Revizyonlar içinde RevisionInsertDelete öğesini bulun
            foreach (RevisionLog revisionLog in revisions)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Type özelliği değerini gösterin
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);

                        // Type özelliğinin kullanımını göster
                        if (revisionInsertDelete.Type == RevisionType.InsertDelete)
                        {
                            Console.WriteLine("This revision represents an insert/delete operation");
                            Console.WriteLine("Affected cell area: " + revisionInsertDelete.CellArea);
                            Console.WriteLine("Action type: " + revisionInsertDelete.ActionType);
                        }

                        break;
                    }
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionInsertDeletePropertyTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


