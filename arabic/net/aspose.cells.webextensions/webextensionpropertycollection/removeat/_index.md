---
title: "WebExtensionPropertyCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WebExtensionPropertyCollection. إزالة الخاصية بالاسم"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionpropertycollection/removeat/
---
## WebExtensionPropertyCollection.RemoveAt method

يزيل الخاصية حسب الاسم.

```csharp
public void RemoveAt(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة خصائص web extension
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // إضافة بعض الخصائص إلى المجموعة
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");
            properties.Add("Property3", "Value3");

            try
            {
                // استدعاء طريقة RemoveAt مع معلمة string
                properties.RemoveAt("Property2");

                Console.WriteLine("Property with name 'Property2' removed successfully.");
                
                // عرض الخصائص المتبقية
                Console.WriteLine("Remaining properties:");
                for (int i = 0; i < properties.Count; i++)
                {
                    Console.WriteLine($"{properties[i].Name}: {properties[i].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("WebExtensionPropertyCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


