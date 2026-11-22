---
title: "NameCollection.Remove"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة NameCollection. إزالة مصفوفة من الأسماء"
type: docs
url: /ar/net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

إزالة مصفوفة من الأسماء

```csharp
public void Remove(string[] names)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الأسماء | String[] | نص الأسماء. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الحصول على NameCollection من المصنف
            NameCollection names = workbook.Worksheets.Names;
            
            // إضافة بعض النطاقات المسماة لتوضيح الإزالة
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // تحضير مصفوفة الأسماء للإزالة
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // استدعاء طريقة Remove مع معامل String[]
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // عرض الأسماء المتبقية
                Console.WriteLine("\nRemaining names in the collection:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

إزالة الاسم.

```csharp
public void Remove(string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص الاسم. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة نطاق مسمى
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
            range.Name = "TestRange";
            
            // عرض العدد قبل الإزالة
            Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
            
            // إزالة النطاق المسمى
            workbook.Worksheets.Names.Remove("TestRange");
            
            // عرض العدد بعد الإزالة
            Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
        }
    }
}
```

### انظر أيضًا

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


