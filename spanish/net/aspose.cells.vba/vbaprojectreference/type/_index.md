---
title: "VbaProjectReference.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProjectReference. Obtiene el tipo de esta referencia"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Obtiene el tipo de esta referencia.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Inicializar proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Agregar una referencia registrada al proyecto VBA
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Obtener la primera referencia y demostrar la propiedad Type
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);

            // Guarda el libro de trabajo
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");
        }
    }
}
```

### Ver también

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


