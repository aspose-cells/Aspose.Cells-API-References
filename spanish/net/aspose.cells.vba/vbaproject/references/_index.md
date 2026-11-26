---
title: "VbaProject.References"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Obtiene todas las referencias del proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

Obtiene todas las referencias del proyecto VBA.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyReferencesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo (el proyecto VBA se crea automáticamente para archivos .xlsm)
            Workbook workbook = new Workbook();
            
            // Acceder a las referencias del proyecto VBA (solo disponible si el libro tiene proyecto VBA)
            if (workbook.VbaProject != null)
            {
                VbaProjectReferenceCollection references = workbook.VbaProject.References;
                
                // Agregar diferentes tipos de referencias
                references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
                references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
                references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");

                // Mostrar el recuento de referencias
                Console.WriteLine($"Total references: {references.Count}");
            }

            // Guardar como libro de trabajo habilitado para macros
            workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


