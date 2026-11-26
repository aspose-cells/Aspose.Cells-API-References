---
title: "Перечисление SheetType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.SheetType. Указывает тип листа"
type: docs
url: /ru/net/aspose.cells/sheettype/
---
## SheetType enumeration

Указывает тип листа.

```csharp
public enum SheetType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| VB | `0` | Модуль Visual Basic |
| Worksheet | `1` |  |
| Chart | `2` | Диаграмма |
| BIFF4Macro | `3` | Лист макросов BIFF4 |
| InternationalMacro | `4` | Международный лист макросов |
| Other | `5` |  |
| Dialog | `6` | Лист диалога |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSheetTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Вставить новый лист типа Worksheet по индексу 0
            Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            
            // Установить имя нового листа
            newWorksheet.Name = "InsertedSheet";
            
            // Получить доступ к ячейкам нового листа и добавить некоторые данные
            newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
            
            // Сохраните книгу
            workbook.Save("SheetTypeDemoOutput.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


