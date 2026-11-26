---
title: "ListObjectCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListObjectCollection. Добавляет ListObject в лист"
type: docs
url: /ru/net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Добавляет объект ListObject в лист.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startRow | Int32 | Начальная строка диапазона списка. |
| startColumn | Int32 | Начальная строка диапазона списка. |
| endRow | Int32 | Начальная строка диапазона списка. |
| endColumn | Int32 | Начальная строка диапазона списка. |
| hasHeaders | Boolean | Наличие заголовков в диапазоне. |

### Возвращаемое значение

Индекс нового ListObject

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить данные в диапазоне
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1", "Col2", "Col3"},
                {100, 200, 300}
            };

            // Добавить ListObject, используя метод Add с параметрами Int32
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount - 1;
            int endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Включить итоговые значения и задать формулу для одного столбца
            worksheet.ListObjects[0].ShowTotals = true;
            worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";

            // Сохраните книгу
            workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Добавляет объект ListObject в лист.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startCell | String | Начальная ячейка диапазона списка. |
| endCell | String | Конечная ячейка диапазона списка. |
| hasHeaders | Boolean | Наличие заголовков в диапазоне. |

### Возвращаемое значение

Индекс нового ListObject

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить примерными данными
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);

            // Добавить объект списка, используя строковые ссылки на диапазон
            ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add("A1", "B3", true);
            
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### См. также

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


