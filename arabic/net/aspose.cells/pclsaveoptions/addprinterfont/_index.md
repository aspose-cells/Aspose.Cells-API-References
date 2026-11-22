---
title: "PclSaveOptions.AddPrinterFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PclSaveOptions. تضيف معلومات حول الخط الذي تم إضافته بالفعل إلى الطابعة من قبل الشركة المصنعة"
type: docs
url: /ar/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

يضيف معلومات حول الخط الذي تم إضافته بالفعل إلى الطابعة من قبل الشركة المصنعة.

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fontFullName | String | الاسم الكامل للخط (مثال: "Times New Roman Bold Italic") المستخدم في ملف المصدر. |
| fontPclName | String | اسم الخط الذي سيُستخدم في مستند Pcl الناتج. |

### ملاحظات

هناك 52 خطًا يجب تضمينها في أي طابعة وفقًا لمواصفات Pcl. ومع ذلك يمكن للمصنعين إضافة خطوط أخرى إلى أجهزتهم.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض النص إلى ورقة العمل لتوضيح استخدام الخط.
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // إنشاء خيارات حفظ PCL
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // استدعِ طريقة AddPrinterFont بأسماء خطوط محددة.
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // احفظ المصنف باستخدام خيارات PCL.
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


