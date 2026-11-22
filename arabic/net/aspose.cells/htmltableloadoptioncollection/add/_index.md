---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة HtmlTableLoadOptionCollection. تضيف HtmlTableLoadOption واحد إلى هذه المجموعة"
type: docs
url: /ar/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

يضيف HtmlTableLoadOption واحد إلى هذه المجموعة.

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عنصر | HtmlTableLoadOption | واحد HtmlTableLoadOption |

### قيمة الإرجاع

فهرس العنصر المضاف

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة AddTableLoadOption(). سيتم إزالة هذه الطريقة بعد 6 أشهر منذ ديسمبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // إضافة خيارات تحميل الجدول
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // تحميل دفتر العمل مع الخيارات
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // حفظ الناتج
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

أضف HtmlTableLoadOption إلى القائمة.

```csharp
public int Add(int tableIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| tableIndex | Int32 | مؤشر الجدول |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // الوصول إلى مثال HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // إضافة HtmlTableLoadOption جديد حسب فهرس الجدول
            int index = tableLoadOptions.Add(0);

            // الوصول إلى HtmlTableLoadOption المضافة
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // إنشاء دفتر عمل وتحميل HTML مع الخيارات
            Workbook workbook = new Workbook("input.html", loadOptions);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

أضف HtmlTableLoadOption إلى القائمة.

```csharp
public int Add(string tableId)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| tableId | String | معرّف الجدول |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // إنشاء HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // الوصول إلى مثال HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // إضافة HtmlTableLoadOption جديد حسب معرف الجدول
            int index = tableLoadOptions.Add("mainTable");

            // الوصول إلى HtmlTableLoadOption المضافة
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // إنشاء دفتر عمل وتحميل HTML مع الخيارات
            Workbook workbook = new Workbook("input.html", loadOptions);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

أضف HtmlTableLoadOption إلى القائمة.

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| tableIndex | Int32 | مؤشر الجدول |
| targetSheetIndex | Int32 | المؤشر المستهدف لورقة العمل في Excel |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // إضافة جداول حسب الفهرس مع مؤشر الورقة المستهدف
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // تحميل ملف HTML باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

أضف HtmlTableLoadOption إلى القائمة.

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| tableId | String | معرّف الجدول |
| targetSheetIndex | Int32 | المؤشر المستهدف لورقة العمل في Excel |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // إنشاء HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // الوصول إلى مثال HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // إضافة HtmlTableLoadOption جديد حسب معرف الجدول وفهرس الورقة المستهدفة
            int index = tableLoadOptions.Add("tableId", 1);

            // إنشاء دفتر عمل وتحميل HTML مع الخيارات
            Workbook workbook = new Workbook("input.html", loadOptions);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

أضف HtmlTableLoadOption إلى القائمة.

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| tableIndex | Int32 | مؤشر الجدول |
| targetSheetIndex | Int32 | المؤشر المستهدف لورقة العمل في Excel |
| originalSheetIndex | Int32 | المؤشر الأصلي لورقة العمل في HTML |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // الوصول إلى HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // إضافة جدول بالفهرس 1، ومؤشر الورقة المستهدف 1، والمؤشر الأصلي للورقة 0
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // إنشاء دفتر عمل وتحميل HTML مع الخيارات
            Workbook workbook = new Workbook("input.html", loadOptions);

            // حفظ النتيجة
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

أضف HtmlTableLoadOption إلى القائمة.

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| tableId | String | معرّف الجدول |
| targetSheetIndex | Int32 | المؤشر المستهدف لورقة العمل في Excel |
| originalSheetIndex | Int32 | المؤشر الأصلي لورقة العمل في HTML |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // عرض طريقة Add مع معلمات (String, Int32, Int32)
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // تحميل ملف HTML (استبدل بمسار الملف الفعلي)
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


