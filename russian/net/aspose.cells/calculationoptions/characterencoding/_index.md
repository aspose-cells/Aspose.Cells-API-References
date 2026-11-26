---
title: "CalculationOptions.CharacterEncoding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CalculationOptions. Указывает кодировку, используемую для кодирования/декодирования символов при вычислении формул. Для функций, таких как CHAR и CODE, полученный результат зависит от региональных настроек и кодировки по умолчанию в среде. С помощью этого свойства пользователь может задать правильную кодировку, используемую этими функциями, чтобы получить ожидаемый результат."
type: docs
url: /ru/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

Указывает кодировку, используемую для кодирования/декодирования символов при вычислении формул. Для функций, таких как CHAR, CODE, результат вычисления зависит от региональных настроек и кодовой страницы среды по умолчанию. С помощью этого свойства пользователь может задать правильную кодировку, используемую этими функциями, чтобы получить ожидаемый результат.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### См. также

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


