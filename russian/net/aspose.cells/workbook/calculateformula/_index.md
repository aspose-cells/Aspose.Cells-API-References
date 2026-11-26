---
title: "Workbook.CalculateFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Вычисляет результат формул"
type: docs
url: /ru/net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

Вычисляет результат формул.

```csharp
public void CalculateFormula()
```

### Примечания

Для всех поддерживаемых формул, пожалуйста, смотрите список по адресу https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Установить значения и формулы
            cells["A1"].PutValue(5);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=B1+10";
            
            // Вычислить формулы
            workbook.CalculateFormula();
            
            // Отобразить результаты
            Console.WriteLine("A1 value: " + cells["A1"].IntValue);
            Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
            Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

Вычисляет результат формул.

```csharp
public void CalculateFormula(bool ignoreError)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ignoreError | Boolean | Указывает, скрывать ли ошибку при вычислении формул. Ошибка может быть вызвана неподдерживаемой функцией, внешними ссылками и т.д. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к первому листу и его ячейкам
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Поместить значения в первую строку (A1:E1)
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(i + 1); // Values 1-5
            }

            // Поместить значения во вторую строку (A2:E2)
            for (int i = 0; i < 5; i++)
            {
                cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
            }

            // Установить общую формулу HLOOKUP в четвертой строке (A4:E4)
            cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);

            // Вычислить формулы без рекурсивного расчёта
            wb.CalculateFormula(false);

            // Отобразите результаты
            Console.WriteLine("Formula calculation results:");
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions) {#calculateformula_1}

Вычисление формул в этой рабочей книге.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | CalculationOptions | Параметры расчёта |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithCalculationOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Создать таблицу и задать имена столбцов
            sheet.Cells["A1"].PutValue("A");
            sheet.Cells["B1"].PutValue("B");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(2);
            
            // Установить формулы и вычислить
            Cells cells = sheet.Cells;
            cells["C1"].PutValue("InvalidColumn");
            cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
            cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
            
            // Вычислить формулы с параметрами
            wb.CalculateFormula(new CalculationOptions());
            
            // Вывести результаты
            Console.WriteLine("D1 result: " + cells["D1"].StringValue);
            Console.WriteLine("E1 result: " + cells["E1"].StringValue);
        }
    }
}
```

### См. также

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


