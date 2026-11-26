---
title: "ListObject.PutCellValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListObject. Помещает значение в ячейку"
type: docs
url: /ru/net/aspose.cells.tables/listobject/putcellvalue/
---
## PutCellValue(int, int, object) {#putcellvalue}

Поместить значение в ячейку.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение строки в таблице. |
| columnOffset | Int32 | Смещение столбца в таблице. |
| значение | Object | Значение ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["C2"].PutValue(300);

            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Продемонстрировать PutCellValue с параметрами Int32, Int32, Object
            listObject.PutCellValue(1, 0, 500); // Update row 1, column 0 with value 500
            listObject.PutCellValue(1, 1, "Updated Value"); // Update row 1, column 1 with string
            listObject.PutCellValue(1, 2, DateTime.Now); // Update row 1, column 2 with current date

            // Сохраните книгу
            workbook.Save("ListObjectPutCellValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellValue(int, int, object, bool) {#putcellvalue_1}

Поместить значение в ячейку.

```csharp
public void PutCellValue(int rowOffset, int columnOffset, object value, bool isTotalsRowLabel)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowOffset | Int32 | Смещение строки в таблице. |
| columnOffset | Int32 | Смещение столбца в таблице. |
| значение | Object | Значение ячейки. |
| isTotalsRowLabel | Boolean | Указывает, является ли это меткой для строки итогов, работает только для строки итогов. Если False и эта строка является строкой итогов, будет вставлена новая строка. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellValueWithInt32Int32ObjectBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для создания ListObject
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Создать ListObject
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // Используйте PutCellValue, чтобы обновить ячейку (строка 2, столбец 1) новым значением и расширить таблицу
            listObject.PutCellValue(2, 1, "Updated Value", true);
            
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


