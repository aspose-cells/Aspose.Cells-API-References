---
title: "JsonLayoutOptions.DateFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonLayoutOptions. تحصل وتضبط تنسيق قيمة التاريخ"
type: docs
url: /ar/net/aspose.cells.utility/jsonlayoutoptions/dateformat/
---
## JsonLayoutOptions.DateFormat property

يحصل على ويضبط تنسيق قيمة التاريخ.

```csharp
public string DateFormat { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تكوين خيارات استيراد JSON مع تنسيق تاريخ مخصص
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = true;
            layoutOptions.ConvertNumericOrDate = true;
            layoutOptions.DateFormat = "DD-MM-YYYY";

            // استيراد بيانات JSON مع قيم التاريخ
            string jsonData = "{\"date\":\"15-05-2023\",\"name\":\"John Doe\"}";
            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);

            // تحقق من أن التاريخ تم استيراده بالتنسيق الصحيح
            Cell dateCell = worksheet.Cells["A2"];
            Console.WriteLine("Imported date value: " + dateCell.StringValue);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


