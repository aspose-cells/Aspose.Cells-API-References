---
title: "Style.InvariantCustom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Возвращает независимую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному числу."
type: docs
url: /ru/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Получает независимую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному числу.

```csharp
public string InvariantCustom { get; }
```

### Примечания

Для встроенных числовых форматов возвращаемое содержимое шаблона всё ещё зависит от культуры, например, для некоторых локалей оно возвращает \"m/d/y\", а для других локалей — \"d/m/y\". Отличие от [`CultureCustom`](../culturecustom/) заключается в (это также то, что означает независимость от культуры): спецификаторы формата и разделители сохраняются как стандартные, например, '/' всегда будет использоваться как разделитель даты и времени, а \"y\" всегда будет использоваться как часть \"год\", независимо от того, какой другой специальный символ используется для конкретной локали.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyInvariantCustomDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            
            // Установить формат даты и значение
            style.Number = 14; // Date format
            style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);

            // Вывести результаты
            Console.WriteLine("Formatted value: " + cell.StringValue);
            Console.WriteLine("CultureCustom: " + style.CultureCustom);
            Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


