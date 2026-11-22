---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ConditionalFormattingIcon. يحصل على بيانات الصورة مع إعداد الخلية"
type: docs
url: /ar/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

يحصل على بيانات الصورة مع إعداد الخلية.

```csharp
public byte[] GetImageData(Cell cell)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خلية | خلية | إعداد الخلية. |

### قيمة الإرجاع

يعيد بيانات صورة الأيقونة.

### أمثلة

```csharp
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconMethodGetImageDataWithCellDemo
    {
        public static void Run()
        {
            string outputDir = "Output/";
            Directory.CreateDirectory(outputDir);

            Workbook workbook = new Workbook("example.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            
            ConditionalFormattingIcon icon = worksheet.ConditionalFormattings[0][0].IconSet.CfIcons[0];
            
            Cell targetCell = worksheet.Cells["E1"];
            byte[] imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "E1_icon.png"), imageData);
            
            targetCell = worksheet.Cells["G1"];
            imageData = icon.GetImageData(targetCell);
            File.WriteAllBytes(Path.Combine(outputDir, "G1_icon.png"), imageData);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


