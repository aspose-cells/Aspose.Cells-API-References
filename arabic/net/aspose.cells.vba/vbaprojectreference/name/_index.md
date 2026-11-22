---
title: "VbaProjectReference.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProjectReference. تحصل وتضبط اسم الإشارة"
type: docs
url: /ar/net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

يحصل ويضبط اسم المرجع.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل (يتم إنشاء مشروع VBA تلقائيًا لملفات .xlsm)
            Workbook workbook = new Workbook(FileFormatType.Xlsm);
            
            // إضافة إشارة إلى مشروع VBA
            string referenceName = "MyReference";
            string referencePath = @"C:\Temp\MyLibrary.dll";
            workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);

            // الوصول إلى الإشارة والتحقق منها عبر خاصية Name
            VbaProjectReferenceCollection references = workbook.VbaProject.References;
            for (int i = 0; i < references.Count; i++)
            {
                if (references[i].Name.Equals(referenceName))
                {
                    Console.WriteLine($"Found reference: {references[i].Name}");
                    break;
                }
            }

            // احفظ المصنف
            workbook.Save("VbaProjectReferenceDemo.xlsm");
        }
    }
}
```

### انظر أيضًا

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


