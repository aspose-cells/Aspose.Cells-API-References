---
title: "الفئة CustomXmlPart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Markup.CustomXmlPart. تمثل Custom XML Data Storage Part داخل الحزمة"
type: docs
url: /ar/net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

يمثل جزء تخزين بيانات XML مخصص (بيانات XML مخصصة داخل حزمة).

```csharp
public class CustomXmlPart
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | يحصل أو يضبط محتوى XML لهذا Custom XML Data Storage Part. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | يحصل ويضبط معرف الجزء XML المخصص. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | يحصل أو يضبط محتوى XML لهذا Custom XML Schema Data Storage Part. |

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassCustomXmlPartDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomXmlPartCollection xmlParts = workbook.CustomXmlParts;

            string xmlData = "<root><item>Sample Data</item></root>";
            byte[] dataBytes = Encoding.UTF8.GetBytes(xmlData);

            string originalId = Guid.NewGuid().ToString();
            int index = xmlParts.Add(dataBytes, null);
            CustomXmlPart newPart = xmlParts[index];
            newPart.ID = originalId;

            Console.WriteLine("Original ID: " + originalId);
            Console.WriteLine("Stored ID: " + newPart.ID);

            string newId = Guid.NewGuid().ToString();
            newPart.ID = newId;
            Console.WriteLine("Updated ID: " + newId);

            workbook.Save("output.xlsx");

            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CustomXmlPart retrievedPart = loadedWorkbook.CustomXmlParts.SelectByID(newId);
            Console.WriteLine("Retrieved ID: " + (retrievedPart != null ? retrievedPart.ID : "Not found"));
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


