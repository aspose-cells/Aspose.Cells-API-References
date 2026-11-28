---
title: "RevisionCellChange.OldStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCellChange özelliği. Hücrenin eski stilini alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellchange/oldstyle/
---
## RevisionCellChange.OldStyle property

Hücrenin eski stilini alır.

```csharp
public Style OldStyle { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldStyleDemo
    {
        public static void Run()
        {
            // Revizyon takibi ile yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresi için başlangıç stilini ayarla
            Cell cell = worksheet.Cells["A1"];
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            initialStyle.Font.Color = System.Drawing.Color.Black;
            cell.SetStyle(initialStyle);
            cell.PutValue("Initial Value");

            // Bir revizyon oluşturmak için hücre stilini değiştir
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.Color = System.Drawing.Color.Red;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);
            cell.PutValue("Modified Value");

            // Revizyon günlüklerine erişin
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // Stil değişikliği bilgisini göster
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Style Font: " + cellChange.OldStyle.Font.Name);
                        Console.WriteLine("Old Style Size: " + cellChange.OldStyle.Font.Size);
                        Console.WriteLine("Old Style Color: " + cellChange.OldStyle.Font.Color);
                        Console.WriteLine("New Style Font: " + cellChange.NewStyle.Font.Name);
                        Console.WriteLine("New Style Size: " + cellChange.NewStyle.Font.Size);
                        Console.WriteLine("New Style Color: " + cellChange.NewStyle.Font.Color);

                        // OldStyle özelliğini kullanmayı göster
                        if (cellChange.OldStyle.Font.Name == "Arial")
                        {
                            Console.WriteLine("\nThe cell originally had Arial font");
                        }
                    }
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionCellChangePropertyOldStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


