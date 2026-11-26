---
title: "CalculationData.GetParamText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CalculationData. Возвращает буквальный текст параметра по заданному индексу"
type: docs
url: /ru/net/aspose.cells/calculationdata/getparamtext/
---
## CalculationData.GetParamText method

Получает буквальный текст параметра по заданному индексу.

```csharp
public string GetParamText(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс параметра (нумерация с нуля) |

### Возвращаемое значение

буквальный текст параметра

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamTextWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            sheet.Cells["A1"].Formula = "=SUM(INDIRECT(\"'Book2.xlsx'!Table1[#All]\"))";
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();
            workbook.CalculateFormula(options);
        }
    }

    class CustomCalcEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                Console.WriteLine("SUM parameter: " + data.GetParamText(0));
            }
            else if (data.FunctionName == "INDIRECT")
            {
                Console.WriteLine("INDIRECT parameter: " + data.GetParamText(0));
            }
        }
    }
}
```

### См. также

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


