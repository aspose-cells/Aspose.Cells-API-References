---
title: "Workbook.CustomXmlParts"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تمثل جزء تخزين بيانات XML مخصص Custom XML Data Storage Part داخل الحزمة"
type: docs
url: /ar/net/aspose.cells/workbook/customxmlparts/
---
## Workbook.CustomXmlParts property

يمثل جزء تخزين بيانات XML مخصص (بيانات XML مخصصة داخل حزمة).

```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomXmlPartsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // عرّف بيانات XML والمخطط
            string xmlData = "<MyXmlData1 xmlns=\"http://my.namespace.com\"/>";
            string xmlSchema = "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>" +
                "<ds:datastoreItem ds:itemID=\"{1D3CF2F4-9155-40AE-99F6-33298D217F89}\" xmlns:ds=\"http://schemas.openxmlformats.org/officeDocument/2006/customXml\">" +
                    "<ds:schemaRefs>" +
                        "<ds:schemaRef ds:uri=\"http://my.namespace.com\"/>" +
                    "</ds:schemaRefs>" +
                "</ds:datastoreItem>";

            // أضف جزء XML مخصص إلى المصنف
            wb.CustomXmlParts.Add(Encoding.UTF8.GetBytes(xmlData), Encoding.UTF8.GetBytes(xmlSchema));

            // احفظ وأعد تحميل المصنف
            string outputPath = "output.xlsx";
            wb.Save(outputPath);
            
            Workbook loadedWb = new Workbook(outputPath);
            
            // اعرض عدد أجزاء XML المخصصة
            Console.WriteLine($"Number of custom XML parts: {loadedWb.CustomXmlParts.Count}");
        }
    }
}
```

### انظر أيضًا

* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


