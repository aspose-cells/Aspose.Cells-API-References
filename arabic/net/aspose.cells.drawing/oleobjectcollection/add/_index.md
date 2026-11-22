---
title: "OleObjectCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة OleObjectCollection. تضيف OleObject إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.drawing/oleobjectcollection/add/
---
## Add(int, int, int, int, byte[]) {#add}

يضيف OleObject إلى المجموعة.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الارتفاع | Int32 | ارتفاع oleObject، بوحدة البكسل. |
| العرض | Int32 | عرض oleObject، بوحدة البكسل. |
| imageData | Byte[] | صورة ole object كمصفوفة بايت. |

### قيمة الإرجاع

[`OleObject`](../../oleobject/) object index.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير بيانات كائن OLE (ملف Excel نموذجي كمصفوفة بايت)
            byte[] oleData;
            try
            {
                string sampleFilePath = "sample.xlsx";
                oleData = File.ReadAllBytes(sampleFilePath);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error reading sample file: {ex.Message}");
                return;
            }

            try
            {
                // استدعِ طريقة Add مع المعاملات: (upperLeftRow, upperLeftColumn, height, width, imageData)
                int oleIndex = worksheet.OleObjects.Add(5, 2, 200, 300, oleData);

                Console.WriteLine($"OLE object added successfully at index: {oleIndex}");
                Console.WriteLine($"Position: Row 5, Column 2");
                Console.WriteLine($"Size: 200px height, 300px width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, byte[], string) {#add_1}

يضيف OleObject مرتبط إلى المجموعة.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData, 
    string linkedFile)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الارتفاع | Int32 | ارتفاع oleObject، بوحدة البكسل. |
| العرض | Int32 | عرض oleObject، بوحدة البكسل. |
| imageData | Byte[] | صورة ole object كمصفوفة بايت. |
| linkedFile | String |  |

### قيمة الإرجاع

[`OleObject`](../../oleobject/) object index.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير بيانات كائن OLE
            int upperLeftRow = 1;
            int upperLeftColumn = 1;
            int height = 200;
            int width = 200;
            byte[] imageData = File.ReadAllBytes("sample.ole");
            string linkedFile = "sample.xlsx";

            try
            {
                // استدعِ طريقة Add مع أنواع المعاملات المحددة
                int index = worksheet.OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile);
                
                Console.WriteLine($"OLE object added at index: {index}");
                Console.WriteLine($"Total OLE objects in worksheet: {worksheet.OleObjects.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


