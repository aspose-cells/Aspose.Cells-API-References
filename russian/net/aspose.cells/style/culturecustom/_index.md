---
title: "Style.CultureCustom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает и задает зависящую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроен, будет возвращена строка шаблона, соответствующая встроенному формату."
type: docs
url: /ru/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Получает и задает зависящую от культуры строку шаблона для числового формата. Если для этого объекта не установлен числовой формат, будет возвращено null. Если числовой формат встроенный, будет возвращена строка шаблона, соответствующая встроенному числу.

```csharp
public string CultureCustom { get; set; }
```

### Примечания

Для встроенного числового формата как содержимое шаблона (например, один из встроенных форматов даты — "m/d/y" для некоторых локалей, а для других локалей оно становится "d/m/y"), так и спецификатор формата (например, некоторые локали используют символ, отличный от 'y', для обозначения года в формате даты) зависят от культуры; для пользовательского формата изменяются только спецификаторы формата в соответствии с культурой, остальные части шаблона форматирования не изменяются.

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCultureCustomDemo
    {
        public static void Run()
        {
            // Создайте книгу и установите венгерскую культуру
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo("hu-HU");

            // Получите первую ячейку и её стиль
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();

            // Установите пользовательский формат и продемонстрируйте преобразование CultureCustom
            string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
            string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
            
            style.Custom = customFormat;
            Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
            
            style.CultureCustom = cultureCustomFormat;
            Console.WriteLine("Custom from CultureCustom: " + style.Custom);

            // Примените стиль и продемонстрируйте форматирование с учётом культуры
            cell.SetStyle(style);
            cell.PutValue(47512); // January 29, 2030
            Console.WriteLine("Formatted value: " + cell.StringValue);

            // Продемонстрируйте формулу с учётом культурного форматирования
            cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
            wb.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.StringValue);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


