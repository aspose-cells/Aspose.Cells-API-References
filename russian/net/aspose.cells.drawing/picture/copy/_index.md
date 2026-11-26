---
title: "Picture.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Picture. Копирует изображение"
type: docs
url: /ru/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

Копировать картинку.

```csharp
public void Copy(Picture source, CopyOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| источник | Изображение | Исходное изображение. |
| опции | CopyOptions | Параметры копирования. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodCopyWithPictureCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Вставить первое изображение (используя путь к образцу)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "sample1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            
            // Вставить второе изображение (используя путь к образцу изображения)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "sample2.jpg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            
            // Скопировать изображение 1 в изображение 2 с помощью CopyOptions
            CopyOptions options = new CopyOptions();
            pic2.Copy(pic1, options);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [CopyOptions](../../../aspose.cells/copyoptions/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


