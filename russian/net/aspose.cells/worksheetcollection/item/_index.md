---
title: "WorksheetCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Возвращает элемент Worksheet по указанному индексу"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Возвращает элемент [`Worksheet`](../../worksheet/) по указанному индексу.

```csharp
public Worksheet this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Использование свойства Item для доступа к ячейке
            Cell cell = cells[0, 0];
            cell.Formula = "=SUM(1, 2, 3)";
            
            workbook.CalculateFormula();
            Console.WriteLine("Cell value: " + cell.IntValue);
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Возвращает элемент [`Worksheet`](../../worksheet/) с указанным именем.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Параметр | Описание |
| --- | --- |
| sheetName | Имя листа |

### Возвращаемое значение

Элемент с указанным именем.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Доступ к листам с помощью свойства Item по индексу и имени
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            
            // Доступ к листу по имени с использованием свойства Item
            Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
            
            // Добавьте данные для демонстрации доступа к листу
            Cells cells = accessedSheet.Cells;
            cells["A1"].PutValue("Worksheet accessed successfully!");
            cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Вставьте столбец во второй лист
            workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
            
            // Сохраните книгу
            workbook.Save("WorksheetCollectionItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


