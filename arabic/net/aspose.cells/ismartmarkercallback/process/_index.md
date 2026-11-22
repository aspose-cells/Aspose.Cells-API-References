---
title: "ISmartMarkerCallBack.Process"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ISmartMarkerCallBack. رد نداء لمعالجة علامة ذكية"
type: docs
url: /ar/net/aspose.cells/ismartmarkercallback/process/
---
## ISmartMarkerCallBack.Process method

رد اتصال لمعالجة علامة ذكية.

```csharp
public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | Int32 | فهرس الورقة. |
| rowIndex | Int32 | فهرس الصف. |
| colIndex | Int32 | فهرس العمود. |
| tableName | String | اسم الجدول لعلامة smartmarker. |
| columnName | String | اسم الجدول لعلامة smartmarker. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo : ISmartMarkerCallBack
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo callback = 
                new ISmartMarkerCallBackMethodProcessWithInt32Int32Int32StringStringDemo();

            try
            {
                // استدعِ طريقة Process مع معلمات نموذجية
                callback.Process(0, 5, 3, "Products", "ProductName");
                
                Console.WriteLine("Process method executed successfully with parameters (0, 5, 3, \"Products\", \"ProductName\")");
                
                // تعيين قيمة لإظهار التأثير
                worksheet.Cells[5, 3].PutValue("ProcessedValue");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
            
            workbook.Save("ISmartMarkerCallBackProcessDemo.xlsx");
        }

        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // تنفيذ طريقة Process
            Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}, Table: {tableName}, ColumnName: {columnName}");
        }
    }
}
```

### انظر أيضًا

* interface [ISmartMarkerCallBack](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


