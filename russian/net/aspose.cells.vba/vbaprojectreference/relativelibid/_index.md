---
title: "VbaProjectReference.RelativeLibid"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProjectReference. Получает и задает идентификатор ссылочного VBA проекта с относительным путем"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreference/relativelibid/
---
## VbaProjectReference.RelativeLibid property

Получает и задает идентификатор ссылочного проекта VBA с относительным путем.

```csharp
public string RelativeLibid { get; set; }
```

### Примечания

Только для ссылки на проект.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyRelativeLibidDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            VbaProject vbaProject = workbook.VbaProject;

            int referenceIndex = vbaProject.References.AddProjectRefrernce("MyReference", null, "..\\lib\\OriginalReference.xlam");
            VbaProjectReference reference = vbaProject.References[referenceIndex];

            Console.WriteLine("Current RelativeLibid value: " + reference.RelativeLibid);

            reference.RelativeLibid = "..\\new_lib\\ModifiedReference.xlam";

            Console.WriteLine("Updated RelativeLibid value: " + reference.RelativeLibid);

            workbook.Save("PropertyRelativeLibidDemo.xlsx");
        }
    }
}
```

### См. также

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


