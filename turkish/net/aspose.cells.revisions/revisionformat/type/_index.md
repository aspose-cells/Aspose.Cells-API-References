---
title: "RevisionFormat.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionFormat özelliği. Revizyon tipini alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

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

    public class RevisionFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Revizyon izlemeyi etkinleştirmek için paylaşımlı modda yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir revizyon oluşturmak için bazı veriler ekleyin ve biçimlendirme uygulayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // Biçim revizyonu oluşturmak için bir stil uygulayın
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // Revizyon günlüklerine erişin
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Type özelliği değerini gösterin
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // Revizyon hakkında ek bilgi gösterin
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionFormatTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
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
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


