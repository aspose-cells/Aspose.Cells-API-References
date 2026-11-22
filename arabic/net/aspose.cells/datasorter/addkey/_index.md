---
title: "DataSorter.AddKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DataSorter. يضيف فهرس العمود المرتب وترتيب الفرز"
type: docs
url: /ar/net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

يضيف فهرس العمود المرتب وترتيب الفرز.

```csharp
public void AddKey(int key, SortOrder order)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مفتاح | Int32 | فهرس العمود المرتب (الموضع المطلق، العمود A هو 0، B هو 1، ...) |
| ترتيب | SortOrder | ترتيب الفرز |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // أضف مفتاح فرز للعمود B (الفهرس 1) بترتيب تصاعدي
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // رتب نطاق البيانات (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // أخرج القيم المرتبة
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مفتاح | Int32 | فهرس العمود المرتب (الموضع المطلق، العمود A هو 0، B هو 1، ...) |
| ترتيب | SortOrder | ترتيب الفرز. |
| customList | String | قائمة الفرز المخصصة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة للفرز
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // إنشاء مُرتّب البيانات وإضافة مفتاح فرز مخصص
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // فرز البيانات
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // حفظ النتيجة
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مفتاح | Int32 | فهرس العمود المرتب (الموضع المطلق، العمود A هو 0، B هو 1، ...) |
| type | SortOnType | نوع القيمة المرتبة. |
| ترتيب | SortOrder | ترتيب الفرز. |
| customList | Object | قائمة الفرز المخصصة. |

### ملاحظات

إذا كان النوع SortOnType.CellColor أو SortOnType.FontColor، فإن customList هو Color.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // إنشاء مُرتّب بيانات
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // استدعِ AddKey مع المعلمات: (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // تحديد النطاق للفرز
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // فرز البيانات
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مفتاح | Int32 | فهرس العمود المرتب (الموضع المطلق، العمود A هو 0، B هو 1، ...) |
| ترتيب | SortOrder | ترتيب الفرز. |
| customList | String[] | قائمة الفرز المخصصة. |

### انظر أيضًا

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


