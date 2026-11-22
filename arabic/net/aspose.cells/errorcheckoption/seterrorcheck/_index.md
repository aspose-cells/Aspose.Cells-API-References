---
title: "ErrorCheckOption.SetErrorCheck"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ErrorCheckOption. تحدد ما إذا كان نوع الخطأ المعطى سيُفحص"
type: docs
url: /ar/net/aspose.cells/errorcheckoption/seterrorcheck/
---
## ErrorCheckOption.SetErrorCheck method

يضبط ما إذا كان نوع الخطأ المعطى سيُفحص.

```csharp
public void SetErrorCheck(ErrorCheckType errorCheckType, bool isCheck)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| errorCheckType | ErrorCheckType | يمكن فحص نوع الخطأ. |
| isCheck | منطقي | صحيح إذا كان نوع الخطأ المعطى يحتاج إلى الفحص (سيظهر مثلث أخضر للخلية إذا فشل الفحص). |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodSetErrorCheckWithErrorCheckTypeBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("123");
            worksheet.Cells["A2"].PutValue("Sample text for error checking");
            
            // تكوين خيارات فحص الأخطاء
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            
            // عرض SetErrorCheck مع قيم ErrorCheckType مختلفة
            errorCheckOption.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextDate, true);
            errorCheckOption.SetErrorCheck(ErrorCheckType.TextNumber, false);
            
            // تطبيق على كامل ورقة العمل
            errorCheckOption.AddRange(CellArea.CreateCellArea(0, 0, worksheet.Cells.MaxRow, worksheet.Cells.MaxDataColumn));
            
            workbook.Save("ErrorCheckExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ErrorCheckType](../../errorchecktype/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


