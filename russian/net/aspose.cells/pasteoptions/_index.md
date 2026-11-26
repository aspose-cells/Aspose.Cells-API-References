---
title: "Класс PasteOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.PasteOptions. Представляет параметры специальной вставки"
type: docs
url: /ru/net/aspose.cells/pasteoptions/
---
## PasteOptions class

Представляет параметры специальной вставки.

```csharp
public class PasteOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PasteOptions](pasteoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | Игнорировать ссылки на оригинальный файл. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | Сохраняет таблицы в диапазоне назначения. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | True означает копирование только видимых ячеек. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | Получает и задает тип операции при вставке диапазона. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | Тип специальной вставки. |
| [ShiftFormulasOfShapes](../../aspose.cells/pasteoptions/shiftformulasofshapes/) { get; set; } | Указывает, следует ли смещать формулы фигур при копировании диапазонов. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | Указывает, следует ли пропускать пустые ячейки. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | True для транспонирования строк и столбцов при вставке диапазона. Значение по умолчанию — False. |

### Примеры

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsDemo
    {
        public static void PasteOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте некоторые данные в первый лист
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Создайте другой лист
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");

            // Определите исходный диапазон
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");

            // Определите диапазон назначения
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");

            // Создайте объект PasteOptions
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // Скопируйте диапазон с указанными параметрами вставки
            destRange.Copy(sourceRange, pasteOptions);

            // Сохраните книгу
            workbook.Save("PasteOptionsExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


