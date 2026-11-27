---
title: "SqlScriptColumnTypeMap.GetNumbericType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SqlScriptColumnTypeMap‑metod. Hämtar numerisk typ i databasen"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/
---
## SqlScriptColumnTypeMap.GetNumbericType method

Hämtar numerisk typ i databasen.

```csharp
[Obsolete("Use SqlScriptColumnTypeMap.GetNumberType() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetNumbericType()
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd i stället SqlScriptColumnTypeMap.GetNumberType()-metoden. Denna metod kommer att tas bort 6 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en instans av SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Hämta och visa den numeriska typmappningen
            string numericType = columnTypeMap.GetNumbericType();
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Skapa en enkel arbetsbok med numeriska data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue(123.45);

            // Spara med SQL‑skriptalternativ med hjälp av typmappningen
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            workbook.Save("NumericTypeDemo.sql", saveOptions);
        }
    }
}
```

### Se även

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


