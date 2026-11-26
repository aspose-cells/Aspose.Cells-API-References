---
title: "Enumeración VbaProjectReferenceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Vba.VbaProjectReferenceType. Representa el tipo de referencia de proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreferencetype/
---
## VbaProjectReferenceType enumeration

Representa el tipo de referencia del proyecto VBA.

```csharp
public enum VbaProjectReferenceType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Registered | `0` | Especifica una referencia a una biblioteca de tipos de Automatización. |
| Control | `1` | Especifica una referencia a una biblioteca de tipos manipulada y su biblioteca de tipos extendida. |
| Project | `2` | Especifica una referencia a un proyecto VBA externo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceTypeDemo
    {
        public static void VbaProjectReferenceTypeExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Inicializar proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Agregar referencia de proyecto VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Guardando el archivo Excel
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // Demostrando el uso de la enumeración VbaProjectReferenceType
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


