---
title: "الفئة SqlScriptColumnTypeMap"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Saving.SqlScriptColumnTypeMap. تمثل خريطة نوع العمود"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptcolumntypemap/
---
## SqlScriptColumnTypeMap class

يمثل خريطة نوع العمود.

```csharp
public class SqlScriptColumnTypeMap
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SqlScriptColumnTypeMap](sqlscriptcolumntypemap/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [GetNumbericType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/)() | (**Obsolete.**) يحصل على النوع الرقمي في قاعدة البيانات. |
| virtual [GetNumberType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumbertype/)() | يحصل على النوع الرقمي في قاعدة البيانات. |
| virtual [GetStringType](../../aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/)() | يحصل على النوع النصي في قاعدة البيانات. |

### أمثلة

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
            // إنشاء مثيل من SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // عرض استخدام طريقتي GetStringType و GetNumbericType
            string stringType = columnTypeMap.GetStringType();
            string numericType = columnTypeMap.GetNumbericType();

            // إخراج النتائج إلى وحدة التحكم
            Console.WriteLine("String Type in Database: " + stringType);
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // إنشاء مثيل من SqlScriptSaveOptions وتعيين ColumnTypeMap
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };

            // أنشئ مصنفًا وأضف بعض البيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // حفظ المصنف كبرنامج نصي SQL باستخدام خيارات الحفظ
            workbook.Save("SqlScriptExample.sql", saveOptions);

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


