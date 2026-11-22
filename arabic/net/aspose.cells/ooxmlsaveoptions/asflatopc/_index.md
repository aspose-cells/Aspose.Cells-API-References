---
title: "OoxmlSaveOptions.AsFlatOpc"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OoxmlSaveOptions. تشير إلى ما إذا كان الحفظ كملف flat opc يمكن توليده بواسطة Open XML SDK"
type: docs
url: /ar/net/aspose.cells/ooxmlsaveoptions/asflatopc/
---
## OoxmlSaveOptions.AsFlatOpc property

يشير إلى ما إذا كان يتم الحفظ كملف opc مسطح يمكن توليده بواسطة Open XML SDK.

```csharp
public bool AsFlatOpc { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Flat OPC Demo");

            try
            {
                // إنشاء مثيل OoxmlSaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // عرض القيمة الافتراضية لخاصية AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // تعيين AsFlatOpc إلى true
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // حفظ المصنف مع تمكين AsFlatOpc
                workbook.Save("AsFlatOpc_Enabled.xlsx", saveOptions);

                // إنشاء خيارات حفظ أخرى مع تعطيل AsFlatOpc
                OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
                saveOptions2.AsFlatOpc = false;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions2.AsFlatOpc);

                // حفظ المصنف مع تعطيل AsFlatOpc
                workbook.Save("AsFlatOpc_Disabled.xlsx", saveOptions2);

                Console.WriteLine("AsFlatOpc property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


