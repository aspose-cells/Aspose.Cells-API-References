---
title: "WorksheetCollection.GetSheetByCodeName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Получает лист по кодовому имени"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Получает лист по коду имени.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| codeName | String | Кодовое имя листа. |

### Возвращаемое значение

Элемент с указанным кодовым именем.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить листы и задать их кодовые имена
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            sheet1.CodeName = "MainSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.CodeName = "DataSheet";

            // Получить лист по кодовому имени
            Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
            Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");

            // Продемонстрировать использование, записывая в ячейки
            mainSheet.Cells["A1"].PutValue("This is Main Sheet");
            dataSheet.Cells["A1"].PutValue("This is Data Sheet");

            // Сохраните книгу
            workbook.Save("GetSheetByCodeNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


