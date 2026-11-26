---
title: "Style.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Копирует данные из другого объекта стиля"
type: docs
url: /ru/net/aspose.cells/style/copy/
---
## Style.Copy method

Копирует данные из другого объекта стиля

```csharp
public void Copy(Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Исходный объект Style |

### Примечания

Этот метод не копирует имя стиля. Если вы хотите скопировать имя, пожалуйста, вызовите следующий код после копирования стиля: destStyle.Name = style.Name.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCopyWithStyleDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу с образцовыми данными
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Sample Text");
            Style srcStyle = srcWorkbook.CreateStyle();
            srcStyle.Font.Name = "Arial";
            srcStyle.Font.Size = 14;
            srcSheet.Cells["A1"].SetStyle(srcStyle);

            // Создайте целевую книгу
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Скопируйте стиль из источника в назначение
            Style destStyle = destWorkbook.CreateStyle();
            destStyle.Copy(srcStyle);
            
            // Примените скопированный стиль
            destSheet.Cells["B2"].PutValue("Copied Style Text");
            destSheet.Cells["B2"].SetStyle(destStyle);

            // Сохранить результат
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


