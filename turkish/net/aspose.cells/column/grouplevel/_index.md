---
title: "Column.GroupLevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column özelliği. Sütunun grup seviyesini alır"
type: docs
url: /tr/net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Sütunun grup seviyesini alır.

```csharp
public byte GroupLevel { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sütunları grupla (isHidden parametresi false olarak ayarlandı)
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // İlk sütunun grup seviyesini al
            int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
            
            // Grup seviyesini çıktı olarak ver
            Console.WriteLine("Group level of first column: " + groupLevel);
            
            // Çalışma kitabını kaydedin
            workbook.Save("GroupLevelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


