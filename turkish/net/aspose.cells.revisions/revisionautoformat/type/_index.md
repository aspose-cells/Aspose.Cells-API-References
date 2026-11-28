---
title: "RevisionAutoFormat.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionAutoFormat özelliği. Revision'ın tipini alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionautoformat/type/
---
## RevisionAutoFormat.Type property

Revizyonun türünü alır

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

    public class RevisionAutoFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Revizyon takibi ile yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Revizyon günlükleri koleksiyonuna erişin
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                // İlk RevisionAutoFormat örneğini bulun
                RevisionAutoFormat revisionFormat = null;
                foreach (RevisionLog revisionLog in revisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionAutoFormat)
                        {
                            revisionFormat = (RevisionAutoFormat)revision;
                            break;
                        }
                    }
                    if (revisionFormat != null) break;
                }

                if (revisionFormat != null)
                {
                    // Type özelliğini (yalnızca okuma) gösterin
                    RevisionType type = revisionFormat.Type;
                    Console.WriteLine($"Revision type: {type}");
                    
                    // Açıklık için enum değerini göster
                    Console.WriteLine($"Revision type value: {(int)type}");
                }
                else
                {
                    Console.WriteLine("No auto-format revisions found in the workbook");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionAutoFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


