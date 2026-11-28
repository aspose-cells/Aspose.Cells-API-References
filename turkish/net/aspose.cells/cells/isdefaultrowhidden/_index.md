---
title: "Cells.IsDefaultRowHidden"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Satırın varsayılan olarak gizli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cells/isdefaultrowhidden/
---
## Cells.IsDefaultRowHidden property

Satırın varsayılan olarak gizli olup olmadığını gösterir.

```csharp
public bool IsDefaultRowHidden { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHiddenDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Varsayılan satır gizli özelliğini ayarla
            worksheet.Cells.IsDefaultRowHidden = true;
            
            // IsDefaultRowHidden'ın mevcut değerini göster
            Console.WriteLine("IsDefaultRowHidden: " + worksheet.Cells.IsDefaultRowHidden);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


