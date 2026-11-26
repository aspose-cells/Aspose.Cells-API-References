---
title: "Style.SetCustom"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Устанавливает строку пользовательского числового формата ячейки"
type: docs
url: /ru/net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

Устанавливает пользовательскую строку формата числа для ячейки.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пользовательский | String | Строка пользовательского числового формата, должна соответствовать шаблону InvariantCulture. |
| builtinPreference | Boolean | Если указанная строка пользовательского числового формата совпадает с одним из встроенных числовых форматов, соответствующих текущим региональным настройкам, следует ли установить числовой формат как встроенный вместо пользовательского. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodSetCustomWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            
            string customFormat1 = "_(\"$\"* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat1, true);
            Console.WriteLine("Custom format 1 applied. Style number: " + style.Number);

            string customFormat2 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat2, true);
            Console.WriteLine("Custom format 2 applied. Style number: " + style.Number);

            string customFormat3 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* -??_);_(@_)";
            style.SetCustom(customFormat3, true);
            Console.WriteLine("Custom format 3 applied. Style number: " + style.Number);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


