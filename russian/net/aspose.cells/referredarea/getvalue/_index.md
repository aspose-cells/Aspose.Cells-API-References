---
title: "ReferredArea.GetValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ReferredArea. Получает значение ячейки с заданным смещением от верхнего левого угла этой области."
type: docs
url: /ru/net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

Получает значение ячейки с заданным смещением от верхнего левого угла этой области.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение строки от начальной строки этой области. |
| colOffset | Int32 | Смещение столбца от начальной строки этой области. |

### Возвращаемое значение

"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = "=A1";
            
            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                object value = referredAreas[0].GetValue(0, 0);
                Console.WriteLine("Value at (0,0): " + value);
            }
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

Получает значение ячейки с заданным смещением от верхнего левого угла этой области.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение строки от начальной строки этой области. |
| colOffset | Int32 | Смещение столбца от начальной строки этой области. |
| calculateFormulas | Boolean | Нужно ли вычислять её рекурсивно, если указанная ссылка является формулой. |

### Возвращаемое значение

"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(100);
            sheet.Cells["B1"].PutValue(200);

            workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names["TestRange"];
            name.RefersTo = "=Sheet1!$A$1:$B$1";

            ReferredArea ra = name.GetReferredAreas(true)[0];
            object result = ra.GetValue(0, 0, true);

            Console.WriteLine("Obtained value: " + result);
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


