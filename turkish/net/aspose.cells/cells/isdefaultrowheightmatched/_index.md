---
title: "Cells.IsDefaultRowHeightMatched"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Satır yüksekliği ve varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir"
type: docs
url: /tr/net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

Satır yüksekliği ve varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHeightMatchedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // IsDefaultRowHeightMatched özelliğini ayarla ve göster
            cells.IsDefaultRowHeightMatched = true;
            Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");

            // Kaydedilmiş çalışma kitabını yükleyerek özelliği doğrulayın
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
            Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


