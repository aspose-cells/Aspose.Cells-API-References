---
title: "NameCollection.Sort"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة NameCollection. تقوم بفرز الأسماء المعرفة"
type: docs
url: /ar/net/aspose.cells/namecollection/sort/
---
## NameCollection.Sort method

ترتيب الأسماء المعرفة.

```csharp
public void Sort()
```

### ملاحظات

إذا قمت بإنشاء عدد كبير من النطاقات المسماة في ملف Excel، يرجى استدعاء هذه الطريقة بعد إنشاء جميع النطاقات المسماة وقبل الحفظ

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodSortDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الحصول على NameCollection من المصنف
            NameCollection names = workbook.Worksheets.Names;
            
            // إضافة بعض النطاقات المسماة لإظهار الفرز
            names.Add("RangeC");
            names.Add("RangeA");
            names.Add("RangeB");
            
            try
            {
                // عرض الأسماء قبل الفرز
                Console.WriteLine("Names before sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
                
                // استدعاء طريقة Sort
                names.Sort();
                
                // عرض الأسماء بعد الفرز
                Console.WriteLine("\nNames after sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Sort method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("NameCollectionSortDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


