---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConditionalFormattingIcon yöntemi. Hücre ayarıyla görüntü verisini alır"
type: docs
url: /tr/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

Hücrenin ayarıyla görüntü verisini alır.

```csharp
public byte[] GetImageData(Cell cell)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hücre | Hücre | Hücrenin ayarı. |

### Dönüş Değeri

Simgenin görüntü verisini döndürür.

### Örnekler

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

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


