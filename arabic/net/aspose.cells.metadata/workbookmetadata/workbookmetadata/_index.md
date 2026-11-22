---
title: "WorkbookMetadata.WorkbookMetadata"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ WorkbookMetadata. أنشئ كائن البيانات الوصفية"
type: docs
url: /ar/net/aspose.cells.metadata/workbookmetadata/workbookmetadata/
---
## WorkbookMetadata(string, MetadataOptions) {#constructor_1}

إنشاء كائن البيانات الوصفية.

```csharp
public WorkbookMetadata(string fileName, MetadataOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String |  |
| خيارات | MetadataOptions |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodCtorWithStringMetadataOptionsDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xls";
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            
            WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);
            
            Console.WriteLine("WorkbookMetadata created successfully with document properties metadata.");
        }
    }
}
```

### انظر أيضًا

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookMetadata(Stream, MetadataOptions) {#constructor}

إنشاء كائن البيانات الوصفية.

```csharp
public WorkbookMetadata(Stream stream, MetadataOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream |  |
| خيارات | MetadataOptions |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.IO;
    using Aspose.Cells;
    using Aspose.Cells.Metadata;

    public class WorkbookMetadataMethodSharpctorWithStreamMetadataOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // أنشئ دفتر عمل بسيط في الذاكرة
                Workbook workbook = new Workbook();
                workbook.Worksheets[0].Cells["A1"].Value = "Sample data";

                // احفظ دفتر العمل إلى تدفق الذاكرة
                using (MemoryStream stream = new MemoryStream())
                {
                    workbook.Save(stream, SaveFormat.Xlsx);
                    stream.Position = 0; // Reset for reading

                    // أنشئ MetadataOptions (باستخدام خصائص المستند كمثال)
                    MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                    // ----- عرض #ctor(Stream, MetadataOptions) -----
                    WorkbookMetadata metadata = new WorkbookMetadata(stream, options);

                    // الوصول إلى مجموعة خصائص المستند المدمجة (للقراءة فقط)
                    var builtInProps = metadata.BuiltInDocumentProperties;
                    Console.WriteLine("Built‑in document properties collection retrieved.");

                    // احفظ البيانات الوصفية إلى ملف جديد (اختياري)
                    metadata.Save("MetadataFromStream.xlsx");
                }

                Console.WriteLine("WorkbookMetadata created and saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during WorkbookMetadata #ctor demo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


