---
title: "ExternalLinkCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ExternalLinkCollection. تضيف رابطًا خارجيًا"
type: docs
url: /ar/net/aspose.cells/externallinkcollection/add/
---
## Add(string, string[]) {#add_1}

يضيف رابطًا خارجيًا.

```csharp
public int Add(string fileName, string[] sheetNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم الملف الخارجي. |
| sheetNames | String[] | جميع أسماء الأوراق في الملف الخارجي. |

### قيمة الإرجاع

موضع الاسم الخارجي في هذه القائمة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على مجموعة الروابط الخارجية
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // تحضير المعلمات لطريقة Add
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // استدعاء طريقة Add مع معلمات (String, String[])
                int index = externalLinks.Add(fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");

                // عرض معلومات الرابط الخارجي المضاف
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link file: {link.DataSource}");
                Console.WriteLine("Referenced sheets:");
                foreach (string sheet in sheetNames)
                {
                    Console.WriteLine($"- {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DirectoryType, string, string[]) {#add}

إضافة رابط خارجي.

```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| directoryType | DirectoryType | نوع الدليل لاسم الملف. |
| fileName | String | اسم الملف. |
| sheetNames | String[] | جميع أسماء الأوراق في الملف الخارجي. |

### قيمة الإرجاع

موضع الاسم الخارجي في هذه القائمة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على مجموعة الروابط الخارجية
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // تحضير المعلمات لطريقة Add
            DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // استدعاء طريقة Add مع معلمات (DirectoryType, String, String[])
                int index = externalLinks.Add(directoryType, fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");
                
                // عرض معلومات حول الرابط الخارجي المضاف
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link references: {link.DataSource}");
                foreach (string sheet in sheetNames) // Changed from link.SheetNames to sheetNames
                {
                    Console.WriteLine($" - References sheet: {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


