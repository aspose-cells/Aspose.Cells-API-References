---
title: "Cells.Find"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Находит ячейку, содержащую входной объект"
type: docs
url: /ru/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Находит ячейку, содержащую входной объект.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| что | Object | Объект для поиска. Тип должен быть int,double,DateTime,string,bool. |
| previousCell | Ячейка | Предыдущая ячейка с тем же объектом. Этот параметр можно установить в null, если поиск начинается с начала. |

### Возвращаемое значение

Объект ячейки.

### Примечания

Возвращает null (Nothing), если ячейка не найдена.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Найдите ячейку, содержащую "Orange"
            Cell searchCell = null;
            Cell foundCell = worksheet.Cells.Find("Orange", searchCell);

            if (foundCell != null)
            {
                Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
                
                // Создайте и примените стиль к найденной ячейке
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                style.Font.IsBold = true;
                foundCell.SetStyle(style);
            }

            // Сохраните книгу
            workbook.Save("FindMethodDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Находит ячейку, содержащую входной объект.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| что | Object | Объект для поиска. Тип должен быть int,double,DateTime,string,bool. |
| previousCell | Ячейка | Предыдущая ячейка с тем же объектом. Этот параметр можно установить в null, если поиск начинается с начала. |
| findOptions | FindOptions | Параметры поиска |

### Возвращаемое значение

Объект ячейки.

### Примечания

Возвращает null (Nothing), если ячейка не найдена.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellFindOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить примерные данные
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["A2"].PutValue("def");
            worksheet.Cells["A3"].PutValue("abc ");
            
            // Создайте параметры поиска
            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Найдите ячейку со значением "abc "
            Cell foundCell = worksheet.Cells.Find("abc ", null, options);
            
            Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
        }
    }
}
```

### См. также

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


