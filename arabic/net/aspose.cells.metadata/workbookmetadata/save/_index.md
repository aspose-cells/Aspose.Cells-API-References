---
title: "WorkbookMetadata.Save"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookMetadata. احفظ البيانات الوصفية المعدلة إلى الملف"
type: docs
url: /ar/net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

احفظ البيانات الوصفية المعدلة إلى الملف.

```csharp
public void Save(string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم الملف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // إنشاء بيانات وصفية جديدة لدفتر العمل
            WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
            
            // إضافة خصائص مخصصة
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            
            // حفظ باستخدام مسار نصي
            doc.Save("output.xlsb");
            
            // تحقق من الملف المحفوظ
            Workbook workbook = new Workbook("output.xlsb");
            Console.WriteLine("File saved successfully with custom properties.");
            Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
        }
    }
}
```

### انظر أيضًا

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

احفظ البيانات الوصفية المعدلة إلى التدفق.

```csharp
public void Save(Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | التدفق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.IO;
    using Aspose.Cells;
    using Aspose.Cells.Metadata;

    public class WorkbookMetadataMethodSaveWithStreamDemo
    {
        public static void Run()
        {
            try
            {
                // مسار إلى دفتر عمل موجود (تأكد من وجود الملف في مجلد التنفيذ)
                string sourcePath = "Sample.xlsx";

                // إنشاء MetadataOptions لخصائص المستند
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // إنشاء نسخة من WorkbookMetadata باستخدام ملف المصدر والخيارات
                WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);

                // الوصول إلى مجموعة خصائص المستند المدمجة (للقراءة فقط)
                var builtInProperties = metadata.BuiltInDocumentProperties;
                Console.WriteLine("Built‑in document properties collection retrieved.");

                // حفظ البيانات الوصفية إلى ملف جديد باستخدام تدفق
                using (FileStream outputStream = new FileStream("MetadataOutput.xlsx",
                                                              FileMode.Create,
                                                              FileAccess.Write))
                {
                    metadata.Save(outputStream);
                }

                Console.WriteLine("Metadata saved successfully to stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during metadata Save: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


