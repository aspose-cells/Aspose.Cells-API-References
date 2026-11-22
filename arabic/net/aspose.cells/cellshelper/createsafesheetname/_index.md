---
title: "CellsHelper.CreateSafeSheetName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تتحقق من اسم الورقة المعطى وتُنشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المعطى يتوافق مع قواعد أسماء أوراق Excel فستُرجعه. وإلا سيتم قص السلسلة إذا تجاوز طولها الحد المسموح وستُستبدل الأحرف غير الصالحة بـ   ثم تُرجع قيمة السلسلة المعاد بناؤها"
type: docs
url: /ar/net/aspose.cells/cellshelper/createsafesheetname/
---
## CreateSafeSheetName(string) {#createsafesheetname}

يتحقق من اسم الورقة المُعطى وينشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المُعطى يتوافق مع قواعد أسماء أوراق Excel، يتم إرجاعه. وإلا سيتم قص السلسلة إذا تجاوز طولها الحد المسموح وسيتم استبدال الأحرف غير الصالحة بـ ' ', ثم إرجاع قيمة السلسلة المعاد بناؤها.

```csharp
public static string CreateSafeSheetName(string nameProposal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| nameProposal | String | اسم الورقة الذي سيُستخدم |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringDemo
    {
        public static void Run()
        {
            string unsafeName = "sheet*/test*/?#";
            string safeName = CellsHelper.CreateSafeSheetName(unsafeName);
            Console.WriteLine("Original name: " + unsafeName);
            Console.WriteLine("Safe name: " + safeName);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateSafeSheetName(string, char) {#createsafesheetname_1}

يتحقق من اسم الورقة المُعطى وينشئ اسمًا صالحًا عند الحاجة. إذا كان اسم الورقة المُعطى يتوافق مع قواعد أسماء أوراق Excel، يتم إرجاعه. وإلا سيتم قص السلسلة إذا تجاوز طولها الحد المسموح وسيتم استبدال الأحرف غير الصالحة بالحرف المُعطى، ثم إرجاع قيمة السلسلة المعاد بناؤها.

```csharp
public static string CreateSafeSheetName(string nameProposal, char replaceChar)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| nameProposal | String | اسم الورقة الذي سيُستخدم |
| replaceChar | محرف | الحرف الذي سيُستخدم لاستبدال الأحرف غير الصالحة في اسم الورقة المحدد |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCreateSafeSheetNameWithStringCharDemo
    {
        public static void Run()
        {
            // المثال 1: إنشاء اسم ورقة آمن باستخدام حرف الاستبدال الافتراضي
            string name1 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#");
            Console.WriteLine("Safe sheet name (default replacement): " + name1);

            // المثال 2: إنشاء اسم ورقة آمن باستخدام حرف استبدال مخصص 'A'
            string name2 = CellsHelper.CreateSafeSheetName("sheet*/test*/?#", 'A');
            Console.WriteLine("Safe sheet name (custom replacement): " + name2);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


