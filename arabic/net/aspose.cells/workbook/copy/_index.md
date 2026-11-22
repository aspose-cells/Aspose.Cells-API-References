---
title: "Workbook.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تنسخ كائن Workbook آخر"
type: docs
url: /ar/net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

ينسخ كائن مصنف آخر.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | المصنف | كائن Workbook المصدر. |
| copyOptions | CopyOptions | خيارات نسخ مصنف آخر. |

### ملاحظات

من السهل جدًا استنساخ ملف Excel.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
    {
        public static void Run()
        {
            // المصنف المصدر مع وحدات ماكرو
            Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
            
            // المصنف الوجهة (فارغ أو موجود)
            Workbook destWorkbook = new Workbook();
            
            // قم بتكوين خيارات النسخ للحفاظ على وحدات الماكرو
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            
            // انسخ المحتويات من المصنف المصدر إلى المصنف الوجهة
            sourceWorkbook.Copy(destWorkbook, options);
            
            // حفظ النتيجة
            destWorkbook.Save("output_with_macros.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

ينسخ البيانات من كائن مصنف مصدر.

```csharp
public void Copy(Workbook source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | المصنف | كائن Workbook المصدر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookDemo
    {
        public static void Run()
        {
            // مسارات ملفات المصدر والإخراج
            string sourceFile = "source.xlsx";
            string outputFile = "output.xlsx";

            // تحميل دفتر العمل المصدر
            Workbook sourceWorkbook = new Workbook(sourceFile);

            // إنشاء دفتر عمل جديد ونسخ المحتويات من المصدر
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Copy(sourceWorkbook);

            // حفظ دفتر العمل المنسوخ
            destinationWorkbook.Save(outputFile);
            
            Console.WriteLine("Workbook copied successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


