---
title: "SqlScriptColumnTypeMap.GetNumbericType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SqlScriptColumnTypeMap yöntemi. Veritabanındaki sayısal türü alır"
type: docs
url: /tr/net/aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/
---
## SqlScriptColumnTypeMap.GetNumbericType method

Veritabanındaki sayısal türü alır.

```csharp
[Obsolete("Use SqlScriptColumnTypeMap.GetNumberType() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetNumbericType()
```

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen SqlScriptColumnTypeMap.GetNumberType() yöntemini kullanın. Bu yöntem Temmuz 2026'dan itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

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
            // SqlScriptColumnTypeMap sınıfının bir örneğini oluşturun
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Sayısal tip eşlemesini al ve görüntüle
            string numericType = columnTypeMap.GetNumbericType();
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Sayısal veri içeren basit bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue(123.45);

            // Tip eşlemesini kullanarak SQL betik seçenekleriyle kaydet
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            workbook.Save("NumericTypeDemo.sql", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


