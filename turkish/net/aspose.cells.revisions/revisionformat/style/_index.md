---
title: "RevisionFormat.Style"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionFormat özelliği. Uygulanan stili alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionformat/style/
---
## RevisionFormat.Style property

Uygulanan stili alır.

```csharp
public Style Style { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun (değişiklik yapıldığında revizyon takibi varsayılan olarak etkinleştirilir)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir revizyon oluşturmak için bazı veri ve biçimlendirme ekleyin
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            
            // Bir stil oluşturun ve hücreye uygulayın
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 12;
            originalStyle.Font.IsBold = true;
            cell.SetStyle(originalStyle);

            // Revizyonlara RevisionLogs aracılığıyla erişin
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                RevisionCollection revisions = revisionLog.Revisions;
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionFormat revisionFormat)
                    {
                        // Revizyondan mevcut stil özelliklerini gösterin
                        Style style = revisionFormat.Style;
                        Console.WriteLine("Revision Style Font: " + style.Font.Name);
                        Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
                        Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);

                        // Not: Style özelliği RevisionFormat içinde yalnızca okunabilir, bu yüzden doğrudan değiştiremeyiz
                        // Biçimlendirmeyi değiştirmek için hücrenin stilini doğrudan değiştirmemiz gerekir
                    }
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionFormatStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


