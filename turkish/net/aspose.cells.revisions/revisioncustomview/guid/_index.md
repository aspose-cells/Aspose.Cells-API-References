---
title: "RevisionCustomView.Guid"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCustomView özelliği. Özel görünümün küresel olarak benzersiz tanımlayıcısını alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncustomview/guid/
---
## RevisionCustomView.Guid property

Özel görünümün küresel olarak benzersiz tanımlayıcısını alır.

```csharp
public Guid Guid { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCustomViewPropertyGuidDemo
    {
        public static void Run()
        {
            // Özel görünüm revizyonları içeren mevcut bir çalışma kitabını aç
            Workbook workbook = new Workbook("example.xlsx");
            
            // Revizyon günlüklerini işle
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision.Type == RevisionType.CustomView)
                    {
                        RevisionCustomView rcv = (RevisionCustomView)revision;
                        Console.WriteLine($"ActionType: {rcv.ActionType}, Guid: {rcv.Guid}");
                    }
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


