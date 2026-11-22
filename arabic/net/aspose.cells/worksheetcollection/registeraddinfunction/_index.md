---
title: "WorksheetCollection.RegisterAddInFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. يضيف دالة الإضافة إلى المصنف"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

يزيل العنصر عند فهرس محدد. (طريقتان)

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| addInFile | String | الملف يحتوي على وظائف الإضافة |
| functionName | String | اسم دالة الإضافة |
| lib | منطقي | ما إذا كان ملف الإضافة المعطى موجودًا في الدليل أو الدليل الفرعي لمكتبة إضافة المصنف. هذه العلامة سارية وتحدث فرقًا عندما يكون addInFile المعطى مسارًا نسبيًا: true يدل على أن المسار نسبي لمكتبة الإضافة وfalse يدل على أن المسار نسبي لهذا المصنف. |

### قيمة الإرجاع

معرّف البيانات التي تحتوي على دالة الإضافة المعطاة

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // احصل على ورقة العمل الأولى
            Worksheet sheet = wb.Worksheets[0];
            
            // حدد مسارات ملفات العينة (يجب أن تكون موجودة في بيئتك)
            string addInFile1 = Path.Combine("AddIns", "MyAddIn1.xlam");
            string addInFile2 = Path.Combine("AddIns", "MyAddIn2.xlam");
            
            // سجّل وظائف الإضافة بمعلمات مختلفة
            int id1 = wb.Worksheets.RegisterAddInFunction(addInFile1, "MY_UDF1", false);
            int id2 = wb.Worksheets.RegisterAddInFunction(addInFile2, "MY_UDF2", true);
            
            // استخدم الدوال المسجلة في الخلايا
            sheet.Cells["A1"].Formula = "=MY_UDF1()";
            sheet.Cells["A2"].Formula = "=MY_UDF2()";
            
            // احفظ المصنف
            wb.Save("RegisterAddInFunctionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

يزيل العنصر عند فهرس محدد. (طريقتان)

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| id | Int32 | معرف البيانات التي تحتوي على وظائف الإضافة، يمكن الحصول عليه من خلال الاستدعاء الأول لـ `RegisterAddInFunction` لنفس ملف الإضافة. |
| functionName | String | اسم دالة الإضافة |

### قيمة الإرجاع

عنوان URL لملف الإضافة الذي يحتوي على وظائف الإضافة

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRegisterAddInFunctionWithInt32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // سجّل أول وظيفة إضافة واحصل على معرفها
            int functionId = workbook.Worksheets.RegisterAddInFunction("externallink1.xlam", "customfunc1", false);
            
            // سجّل وظيفة الإضافة الثانية باستخدام نفس المعرف
            workbook.Worksheets.RegisterAddInFunction(functionId, "customfunc2");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // استخدم الوظائف المسجلة في الصيغ
            cells["A1"].Formula = "=customfunc1()";
            cells["A2"].Formula = "=customfunc2()";
            
            // احفظ المصنف
            workbook.Save("RegisterAddInFunctionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


