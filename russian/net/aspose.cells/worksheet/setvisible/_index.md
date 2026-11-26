---
title: "Worksheet.SetVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Устанавливает параметры видимости"
type: docs
url: /ru/net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

Устанавливает видимые параметры.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isVisible | Boolean | Является ли лист видимым |
| ignoreError | Boolean | Нужно ли игнорировать ошибку, если эта опция недействительна. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить несколько листов
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Установить видимость листов
            // Первый параметр: isVisible — false, чтобы скрыть лист
            // Второй параметр: ignoreError — true, чтобы игнорировать ошибку, если лист нельзя скрыть
            workbook.Worksheets["Sheet2"].SetVisible(false, true);
            workbook.Worksheets["Sheet3"].SetVisible(false, true);

            // Сохраните книгу
            workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


