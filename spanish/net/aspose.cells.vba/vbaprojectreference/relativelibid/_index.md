---
title: "VbaProjectReference.RelativeLibid"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProjectReference. Obtiene y establece el identificador del proyecto VBA referenciado con una ruta relativa"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreference/relativelibid/
---
## VbaProjectReference.RelativeLibid property

Obtiene y establece el identificador del proyecto VBA referenciado con una ruta relativa.

```csharp
public string RelativeLibid { get; set; }
```

### Observaciones

Solo para referencia de proyecto.

### Ejemplos

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

### Ver también

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


