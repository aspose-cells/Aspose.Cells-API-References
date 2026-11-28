---
title: "Worksheet.MoveTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Sayfayı elektronik tabloda başka bir konuma taşır."
type: docs
url: /tr/net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Sayfayı elektronik tabloda başka bir konuma taşır.

```csharp
public void MoveTo(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Hedef sayfa indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodMoveToWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Yeni bir çalışma sayfası ekle ve 1. konuma taşı
            Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
            newWorksheet.MoveTo(1);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


