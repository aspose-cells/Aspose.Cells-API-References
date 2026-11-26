---
title: "Класс CalculationData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CalculationData. Представляет необходимые данные при вычислении одной функции, такие как имя функции, параметры ...и т.д."
type: docs
url: /ru/net/aspose.cells/calculationdata/
---
## CalculationData class

Представляет необходимые данные при вычислении функции, такие как имя функции, параметры, ...etc.

```csharp
public class CalculationData
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Получает или задаёт вычисленное значение для этой функции. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Получает объект Cell, где находится функция. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Получает индекс столбца ячейки, где находится функция. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Получает индекс строки ячейки, где находится функция. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Получает имя функции, которую нужно вычислить. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Получает количество параметров |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Получает объект Workbook, где находится функция. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Получает объект Worksheet, где находится функция. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Получает буквальный текст параметра по заданному индексу. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Получает представленный объект значения параметра по заданному индексу. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Получает значение(я) параметра по заданному индексу. Если параметр представляет собой выражение, которое необходимо вычислить, оно будет вычислено в режиме массива. |

### Примечания

Все объекты, предоставляемые этим классом, предназначены только для "чтения". Пользователь не должен изменять какие-либо данные в Workbook во время процесса вычисления формул, иначе могут возникнуть неожиданные результаты или исключения.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // Подготовьте простой workbook и worksheet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // Поместите некоторые значения, которые будут использоваться в качестве параметров в пользовательской функции
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // Установите формулу, вызывающую пользовательскую функцию
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // Настройте параметры вычисления для использования пользовательского движка
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // Выполните вычисление – пользовательский движок получит экземпляр CalculationData
                workbook.CalculateFormula(options);

                // Выведите результат пользовательской функции
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // Сохраните книгу для полноты
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // Пользовательский движок вычислений, демонстрирующий доступ к членам CalculationData
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Убедитесь, что мы обрабатываем ожидаемую пользовательскую функцию
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // Получите значения параметров (они возвращаются как объекты)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // Преобразуйте параметры в тип double для вычисления
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // Назначьте вычисленный результат
                    data.CalculatedValue = result;

                    // Продемонстрируйте чтение только‑для‑чтения свойств
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


