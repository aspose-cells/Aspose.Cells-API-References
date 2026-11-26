---
title: "FormulaParseOptions.CheckAddIn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormulaParseOptions. Указывает, проверять ли надстройки в существующих внешних ссылках текущей книги для пользовательской функции без внешней ссылки. По умолчанию true. Если пользовательская функция совпадает с одной из надстроек в существующих внешних ссылках, она считается надстройкой."
type: docs
url: /ru/net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

Проверять ли надстройки в существующих внешних ссылках текущей книги для пользовательской функции без внешней ссылки. По умолчанию true (если пользовательская функция совпадает с одной надстройкой в существующих внешних ссылках, то считается этой надстройкой).

```csharp
public bool CheckAddIn { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCheckAddInDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Зарегистрировать функцию‑надстройку
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);

            // Без CheckAddIn=false - формула будет преобразована в формат надстройки
            cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);

            // С CheckAddIn=false - формула остаётся неизменной
            cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
            Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
        }
    }
}
```

### См. также

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


