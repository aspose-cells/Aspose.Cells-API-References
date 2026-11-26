---
title: "CalculationData.GetParamValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CalculationData. Возвращает объект представленного значения параметра по заданному индексу"
type: docs
url: /ru/net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

Получает представленный объект значения параметра по заданному индексу.

```csharp
public object GetParamValue(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс параметра (начиная с 0) |

### Возвращаемое значение

Вычисленное значение параметра.

### Примечания

Для одного параметра:

Если это простое значение, то возвращает само простое значение;

Если это ссылка, то возвращает объект ReferredArea;

Если он ссылается на набор(ы) данных с несколькими значениями, то возвращает массив объектов;

Если это некоторый тип выражения, требующий вычисления, то оно будет вычислено в режиме значения, и обычно будет возвращено единичное значение в соответствии с текущей базой ячейки. Например, если один параметр формулы D2 — A:A+B:B, то будет вычислено и возвращено A2+B2. Однако если этот параметр указан в режиме массива (с помощью [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) или [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), то будет возвращён массив (object[][]), элементы которого — A1+B1, A2+B2, ….

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://localhost:9090\", \"Target\")";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new HyperlinkCalculationEngine();
            workbook.CalculateFormula(options);
        }

        class HyperlinkCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName.Equals("HYPERLINK", StringComparison.OrdinalIgnoreCase))
                {
                    Console.WriteLine("URL Parameter: " + data.GetParamValue(0));
                    Console.WriteLine("Display Text: " + data.GetParamValue(1));
                }
            }
        }
    }
}
```

### См. также

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


