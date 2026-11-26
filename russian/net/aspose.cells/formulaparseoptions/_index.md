---
title: "Класс FormulaParseOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.FormulaParseOptions. Представляет параметры при разборе формулы"
type: docs
url: /ru/net/aspose.cells/formulaparseoptions/
---
## FormulaParseOptions class

Представляет параметры при разборе формулы.

```csharp
public class FormulaParseOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FormulaParseOptions](formulaparseoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CheckAddIn](../../aspose.cells/formulaparseoptions/checkaddin/) { get; set; } | Проверять ли надстройки в существующих внешних ссылках текущей книги для пользовательской функции без внешней ссылки. По умолчанию true (если пользовательская функция совпадает с одной надстройкой в существующих внешних ссылках, то считается этой надстройкой). |
| [CustomFunctionDefinition](../../aspose.cells/formulaparseoptions/customfunctiondefinition/) { get; set; } | Определение для разбора пользовательских функций. |
| [LocaleDependent](../../aspose.cells/formulaparseoptions/localedependent/) { get; set; } | Является ли формула локализованной. По умолчанию false. |
| [Parse](../../aspose.cells/formulaparseoptions/parse/) { get; set; } | Разбирать ли данную формулу. По умолчанию true. Если false, то строка формулы будет оставлена как есть в ячейке, пока пользователь не вызовет другие методы для её разбора или пока данные разбора формулы не потребуются другим операциям, например расчёту формул. |
| [R1C1Style](../../aspose.cells/formulaparseoptions/r1c1style/) { get; set; } | Является ли формула в стиле ссылок R1C1. По умолчанию false. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaParseOptionsDemo
    {
        public static void FormulaParseOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions
            {
                LocaleDependent = true,
                R1C1Style = false,
                CheckAddIn = true,
                Parse = true,
                CustomFunctionDefinition = null // Assuming no custom function definition for this example
            };

            // Добавить формулу в ячейку, используя параметры
            Cell cell = worksheet.Cells["A1"];
            cell.SetFormula("=SUM(B1:B10)", options);

            // Сохраните книгу
            workbook.Save("FormulaParseOptionsExample.xlsx");
            workbook.Save("FormulaParseOptionsExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


