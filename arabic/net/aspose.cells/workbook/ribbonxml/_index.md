---
title: "Workbook.RibbonXml"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تحصل وتعيّن ملف XML الذي يحدد واجهة شريط الأدوات"
type: docs
url: /ar/net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

يحصل على ويضبط ملف XML الذي يحدد واجهة الشريط.

```csharp
public string RibbonXml { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyRibbonXmlDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // عينة XML لشريط الأدوات لتخصيص الشريط
            string ribbonXml = 
                "<customUI xmlns=\"http://schemas.microsoft.com/office/2006/01/customui\">" +
                "  <ribbon>" +
                "    <tabs>" +
                "      <tab id=\"customTab\" label=\"My Tab\">" +
                "        <group id=\"customGroup\" label=\"My Group\">" +
                "          <button id=\"customButton\" label=\"My Button\" size=\"large\" />" +
                "        </group>" +
                "      </tab>" +
                "    </tabs>" +
                "  </ribbon>" +
                "</customUI>";

            // عيّن خاصية RibbonXml
            workbook.RibbonXml = ribbonXml;

            // احفظ المصنف
            workbook.Save("output.xlsm");

            // تحقق من خاصية RibbonXml
            Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


