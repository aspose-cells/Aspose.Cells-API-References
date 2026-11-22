---
title: "WorksheetCollection.AddCopy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. تُضيف ورقة عمل إلى المجموعة وتنسخ البيانات من ورقة عمل موجودة"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة.

```csharp
public int AddCopy(string sheetName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | String | اسم ورقة العمل المصدر. |

### قيمة الإرجاع

[`Worksheet`](../../worksheet/) object index.

### الاستثناءات

| استثناء | شرط |
| --- | --- |
| [CellsException](../../cellsexception/) | يحدد اسم ورقة عمل غير صالح. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل باسم "Original" إلى المصنف
            Worksheet originalSheet = workbook.Worksheets.Add("Original");
            
            // أضف بعض البيانات إلى ورقة العمل الأصلية
            originalSheet.Cells["A1"].PutValue("This is the original sheet");
            
            // أنشئ نسخة من ورقة العمل "Original"
            int copiedIndex = workbook.Worksheets.AddCopy("Original");
            Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
            copiedSheet.Name = "CopiedSheet";
            
            // عدّل الورقة المنسوخة لتظهر أنها نسخة مستقلة
            copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
            
            // احفظ المصنف
            workbook.Save("WorksheetCopyDemo.xlsx");
            
            Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة.

```csharp
public int AddCopy(int sheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | Int32 | فهرس ورقة العمل المصدر. |

### قيمة الإرجاع

[`Worksheet`](../../worksheet/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بعض البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Worksheet");
            
            // أضف نسخة من ورقة العمل الأولى
            workbook.Worksheets.AddCopy(0);
            
            // تحقق من إنشاء النسخة
            Worksheet copiedWorksheet = workbook.Worksheets[1];
            copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

نسخ مجموعة من أوراق العمل.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | Worksheet[] | ورقات العمل المصدر. |
| destSheetNames | String[] | أسماء الأوراق المنسوخة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض أوراق العمل النموذجية
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // ملء بعض البيانات في أوراق العمل
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");

            // تحضير مصفوفة أوراق العمل المصدر
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet2"],
                workbook.Worksheets["Sheet3"]
            };

            // تحضير مصفوفة أسماء الأوراق الوجهة
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet2",
                "CopyOfSheet3"
            };

            try
            {
                // استدعاء طريقة AddCopy مع معلمات (Worksheet[], String[])
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // تحقق من إنشاء النسخ
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


