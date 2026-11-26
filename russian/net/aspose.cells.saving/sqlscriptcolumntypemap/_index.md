---
title: "Класс SqlScriptColumnTypeMap"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Saving.SqlScriptColumnTypeMap. Представляет карту типов столбцов"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptcolumntypemap/
---
## SqlScriptColumnTypeMap class

Представляет отображение типов столбцов.

```csharp
public class SqlScriptColumnTypeMap
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SqlScriptColumnTypeMap](sqlscriptcolumntypemap/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [GetNumbericType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/)() | (**Obsolete.**) Получает числовой тип в базе данных. |
| virtual [GetNumberType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumbertype/)() | Получает числовой тип в базе данных. |
| virtual [GetStringType](../../aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/)() | Получает строковый тип в базе данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptColumnTypeMapDemo
    {
        public static void SqlScriptColumnTypeMapExample()
        {
            // Создайте экземпляр SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Продемонстрируйте использование методов GetStringType и GetNumbericType
            string stringType = columnTypeMap.GetStringType();
            string numericType = columnTypeMap.GetNumbericType();

            // Выведите результаты в консоль
            Console.WriteLine("String Type in Database: " + stringType);
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Создайте экземпляр SqlScriptSaveOptions и задайте ColumnTypeMap
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };

            // Создайте книгу и добавьте некоторые данные
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Сохраните книгу как SQL‑скрипт, используя параметры сохранения
            workbook.Save("SqlScriptExample.sql", saveOptions);

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


