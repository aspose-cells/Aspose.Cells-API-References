---
title: "ConditionalFormattingIcon.GetImageData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ConditionalFormattingIcon. Получает данные изображения с учётом настройки ячейки"
type: docs
url: /ru/net/aspose.cells/conditionalformattingicon/getimagedata/
---
## ConditionalFormattingIcon.GetImageData method

Получает данные изображения с настройкой ячейки.

```csharp
public byte[] GetImageData(Cell cell)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ячейка | Ячейка | Настройка ячейки. |

### Возвращаемое значение

Возвращает данные изображения значка.

### Примеры

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

### См. также

* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


