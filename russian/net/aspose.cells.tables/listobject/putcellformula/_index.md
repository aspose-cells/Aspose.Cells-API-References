---
title: "ListObject.PutCellFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListObject. Помещает формулу в ячейку таблицы"
type: docs
url: /ru/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Поместить формулу в ячейку таблицы.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение строки в таблице. |
| columnOffset | Int32 | Смещение столбца в таблице. |
| формула | String | Формула ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавьте примерные данные для создания таблицы
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // Создайте объект списка (таблица)
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // Добавьте новую строку и задайте значения/формулу
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // Сохраните книгу
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Поместить формулу в ячейку таблицы.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение строки в таблице. |
| columnOffset | Int32 | Смещение столбца в таблице. |
| формула | String | Формула ячейки. |
| isTotalsRowFormula | Boolean |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для создания объекта списка
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Продемонстрировать PutCellFormula
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


