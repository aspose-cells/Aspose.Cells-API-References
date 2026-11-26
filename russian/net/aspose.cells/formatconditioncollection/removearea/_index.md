---
title: "FormatConditionCollection.RemoveArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FormatConditionCollection. Удаляет диапазон ячеек с условным форматированием по индексу"
type: docs
url: /ru/net/aspose.cells/formatconditioncollection/removearea/
---
## RemoveArea(int) {#removearea_1}

Удаляет условно отформатированный диапазон ячеек по индексу.

```csharp
public void RemoveArea(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс диапазона ячеек с условным форматированием, который нужно удалить. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить условное форматирование
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];

            // Добавить области для форматирования
            formatConditionCollection.AddArea(CellArea.CreateCellArea(0, 0, 10, 5)); // First area
            formatConditionCollection.AddArea(CellArea.CreateCellArea(5, 5, 15, 10)); // Second area

            // Добавить условие
            formatConditionCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");

            // Отобразить начальное количество областей (мы знаем, что добавили 2 области)
            Console.WriteLine("Areas before removal: 2");

            // Удалить вторую область (индекс 1)
            formatConditionCollection.RemoveArea(1);

            // Отобразить количество областей после удаления (мы знаем, что удалили 1 область)
            Console.WriteLine("Areas after removal: 1");

            // Сохраните книгу
            workbook.Save("RemoveAreaDemo.xlsx");
        }
    }
}
```

### См. также

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveArea(int, int, int, int) {#removearea}

Удалить условное форматирование в диапазоне.

```csharp
public bool RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Начальная строка (startRow) диапазона. |
| startColumn | Int32 | Начальный столбец (startColumn) диапазона. |
| totalRows | Int32 | Количество строк в диапазоне. |
| totalColumns | Int32 | Количество столбцов в диапазоне. |

### Возвращаемое значение

Возвращает TRUE, эта FormatCondtionCollection должна быть удалена.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            
            int idx = cfc.Add();
            FormatConditionCollection fcc = cfc[idx];
            
            // Добавить начальную область
            CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
            fcc.AddArea(initialArea);
            
            // Добавить условие
            idx = fcc.AddCondition(FormatConditionType.Expression);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "=A1>0";
            fc.Style.Font.Color = Color.Red;
            
            // Продемонстрировать RemoveArea с параметрами Int32
            Console.WriteLine("Before removal - Areas count: " + fcc.Count);
            fcc.RemoveArea(0, 0, 1, 1); // Remove the initial area
            Console.WriteLine("After removal - Areas count: " + fcc.Count);
            
            // Добавить новую область
            CellArea newArea = CellArea.CreateCellArea(1, 1, 1, 1);
            fcc.AddArea(newArea);
            Console.WriteLine("After adding new area - Areas count: " + fcc.Count);
        }
    }
}
```

### См. также

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


