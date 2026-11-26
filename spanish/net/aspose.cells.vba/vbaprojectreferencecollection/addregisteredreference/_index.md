---
title: "VbaProjectReferenceCollection.AddRegisteredReference"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaProjectReferenceCollection. Agregar una referencia a una biblioteca de tipos Automation"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

Agregue una referencia a una biblioteca de tipos de Automatización.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la referencia. |
| libid | String | El identificador de una biblioteca de tipos Automation. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddRegisteredReferenceWithStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder al proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Agregar una referencia registrada a stdole
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsm");
        }
    }
}
```

### Ver también

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


