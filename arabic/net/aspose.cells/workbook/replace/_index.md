---
title: "Workbook.Replace"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تستبدل قيمة خلية بسلسلة جديدة"
type: docs
url: /ar/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

يستبدل قيمة خلية واحدة بسلسلة نصية جديدة.

```csharp
public int Replace(string placeHolder, string newValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| newValue | String | قيمة السلسلة للاستبدال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Apple Orange");
            
            // استبدال جميع تكرارات "Apple" بـ "Mango"
            workbook.Replace("Apple", "Mango");
            
            // احفظ المصنف
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

يستبدل قيمة خلية واحدة بعدد صحيح جديد.

```csharp
public int Replace(string placeHolder, int newValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| newValue | Int32 | قيمة عددية للاستبدال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بعض البيانات النموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("OriginalValue");
            worksheet.Cells["A2"].PutValue("OriginalValue");
            worksheet.Cells["A3"].PutValue("OriginalValue");
            
            // استبدل جميع التكرارات لـ "OriginalValue" بالعدد الصحيح 100
            workbook.Replace("OriginalValue", 100);
            
            // احفظ المصنف
            workbook.Save("ReplacedWorkbook.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

يستبدل قيمة خلية واحدة بقيمة مزدوجة جديدة.

```csharp
public int Replace(string placeHolder, double newValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| newValue | Double | قيمة مزدوجة للاستبدال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ضع بعض البيانات النموذجية في الخلايا
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnotherOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // استبدل النص بقيمة مزدوجة
            double newValue = 100.0;
            workbook.Replace("AnOldValue", newValue);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

يستبدل قيمة خلية واحدة بمصفوفة سلاسل نصية جديدة.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| newValues | String[] | مصفوفة سلاسل لاستبدالها |
| isVertical | منطقي | True - عمودي، False - أفقي |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات النموذجية إلى الخلايا
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // حدد القيم الجديدة للاستبدال بها
            string[] newValues = new string[] { "Tom", "Alice", "Jerry" };
            
            // استبدل جميع التكرارات لـ "AnOldValue" بالقيم الجديدة
            workbook.Replace("AnOldValue", newValues, true);
            
            // احفظ المصنف
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

يستبدل قيم الخلايا بمصفوفة أعداد صحيحة.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| newValues | Int32[] | مصفوفة أعداد صحيحة للاستبدال |
| isVertical | منطقي | True - عمودي، False - أفقي |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات النموذجية إلى الخلايا
            worksheet.Cells["A1"].PutValue("OldValue");
            worksheet.Cells["A2"].PutValue("OldValue");
            worksheet.Cells["A3"].PutValue("OtherValue");
            
            // حدد قيم الاستبدال
            int[] newValues = new int[] { 1, 2, 3 };
            
            // استبدل "OldValue" بمصفوفة الأعداد الصحيحة
            workbook.Replace("OldValue", newValues, true);
            
            // احفظ المصنف
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

يستبدل قيم الخلايا بمصفوفة مزدوجة.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| newValues | Double[] | مصفوفة مزدوجة للاستبدال |
| isVertical | منطقي | True - عمودي، False - أفقي |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDoubleBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("AnOldValue");
            worksheet.Cells["A2"].PutValue("AnOldValue");
            worksheet.Cells["A3"].PutValue("AnOldValue");
            
            // حدد قيم الاستبدال
            double[] newValues = new double[] { 1.23, 2.56, 3.14159 };
            
            // استبدل جميع التكرارات لـ "AnOldValue" بالقيم الجديدة
            workbook.Replace("AnOldValue", newValues, true);
            
            // احفظ المصنف
            workbook.Save("ReplaceDemoOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

يستبدل قيم الخلايا ببيانات من DataTable.

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| insertTable | DataTable | DataTable للاستبدال |

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringDataTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أنشئ DataTable نموذجية
            DataTable dataTable = new DataTable("Customers");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("City", typeof(string));
            
            // أضف بيانات نموذجية إلى DataTable
            dataTable.Rows.Add(1, "John Doe", "New York");
            dataTable.Rows.Add(2, "Jane Smith", "London");
            dataTable.Rows.Add(3, "Mike Johnson", "Paris");
            
            // أضف بعض النص إلى ورقة العمل التي سيتم استبدالها
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("CustomerData");
            
            // استبدل النص بـ DataTable
            workbook.Replace("CustomerData", dataTable);
            
            // احفظ المصنف
            workbook.Save("Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

يستبدل قيم الخلايا ببيانات جديدة.

```csharp
public int Replace(bool boolValue, object newValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| boolValue | منطقي | القيمة المنطقية التي سيتم استبدالها. |
| newValue | Object | قيمة جديدة. يمكن أن تكون سلسلة أو عدد صحيح أو مزدوج أو قيمة DateTime. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithBooleanObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بعض الخلايا بقيم منطقية
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            worksheet.Cells["A3"].PutValue(true);
            
            try
            {
                // استدعِ طريقة Replace لاستبدال جميع القيم 'true' بـ "REPLACED"
                int replacements = workbook.Replace(true, "REPLACED");
                
                Console.WriteLine($"Replaced {replacements} occurrences of 'true' with 'REPLACED'");
                
                // عرض النتائج
                Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("WorkbookMethodReplaceWithBooleanObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

يستبدل قيم الخلايا ببيانات جديدة.

```csharp
public int Replace(int intValue, object newValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| intValue | Int32 | القيمة الصحيحة التي سيتم استبدالها. |
| newValue | Object | قيمة جديدة. يمكن أن تكون سلسلة أو عدد صحيح أو مزدوج أو قيمة DateTime. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodReplaceWithInt32ObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بعض الخلايا بقيم صحيحة لتتم استبدالها
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(100);
            
            try
            {
                // استدعِ طريقة Replace مع المعلمات (Int32, Object)
                int replacements = workbook.Replace(100, "ReplacedValue");
                
                Console.WriteLine($"Replaced {replacements} occurrences of the value 100");
                
                // عرض محتوى ورقة العمل بعد الاستبدال
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("WorkbookMethodReplaceWithInt32ObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

يستبدل قيمة خلية واحدة بسلسلة نصية جديدة.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| placeHolder | String | عنصر نائب للخلية |
| newValue | String | قيمة السلسلة للاستبدال |
| خيارات | ReplaceOptions | خيارات الاستبدال |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false
            };

            int replacedCount = workbook.Replace("Hello", "Hi", options);

            Console.WriteLine($"Replacements made: {replacedCount}");
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ReplaceOptions](../../replaceoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


