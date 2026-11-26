---
title: "SqlScriptColumnTypeMap.GetNumbericType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SqlScriptColumnTypeMap. Получает числовой тип в базе данных"
type: docs
url: /ru/net/aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/
---
## SqlScriptColumnTypeMap.GetNumbericType method

Получает числовой тип в базе данных.

```csharp
[Obsolete("Use SqlScriptColumnTypeMap.GetNumberType() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetNumbericType()
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод SqlScriptColumnTypeMap.GetNumberType(). Этот метод будет удалён через 6 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetNumbericTypeDemo
    {
        public static void Run()
        {
            // Создайте экземпляр SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Получить и отобразить сопоставление числовых типов
            string numericType = columnTypeMap.GetNumbericType();
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Создать простой рабочий лист с числовыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue(123.45);

            // Сохранить с параметрами SQL‑скрипта, используя сопоставление типов
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            workbook.Save("NumericTypeDemo.sql", saveOptions);
        }
    }
}
```

### См. также

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


