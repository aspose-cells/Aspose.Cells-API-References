---
title: "WorksheetCollection.Insert"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorksheetCollection метод. Вставить лист"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

Вставить лист.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс листа |
| sheetType | SheetType | Тип листа. |

### Возвращаемое значение

Возвращает вставленный лист.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
            worksheet.Name = "InsertedSheet";
            workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
            workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

Вставить лист.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс листа |
| sheetType | SheetType | Тип листа. |
| sheetName | String | Имя листа. |

### Возвращаемое значение

Возвращает вставленный лист.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Вставить новый лист с индексом 0 и именем "InsertedSheet"
            workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
            
            // Получить доступ к вставленному листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Поместить некоторые данные в ячейку A1 вставленного листа
            worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
            
            // Сохраните книгу
            workbook.Save("WorksheetInsertDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


