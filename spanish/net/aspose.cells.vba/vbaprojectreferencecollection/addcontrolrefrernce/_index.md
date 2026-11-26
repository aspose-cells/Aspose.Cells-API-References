---
title: "VbaProjectReferenceCollection.AddControlRefrernce"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaProjectReferenceCollection. Añade una referencia a una biblioteca de tipos retorcida y a su biblioteca de tipos extendida"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

Agregue una referencia a una biblioteca de tipos retorcida y a su biblioteca de tipos extendida.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddControlReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la referencia. |
| libid | String | El identificador de una biblioteca de tipos Automation. |
| twiddledlibid | String | El identificador de una biblioteca de tipos retorcida |
| extendedLibid | String | El identificador de una biblioteca de tipos extendida |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método VbaProjectReferenceCollection.AddControlReferernce(). Este método será eliminado 12 meses después desde julio de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddControlRefrernceWithStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            // Añadir referencia de control con todos los parámetros string
            vbaProject.References.AddControlRefrernce(
                "MSForms",
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
                "twiddledLibid",
                "extendedLibid");

            Console.WriteLine("Control reference added successfully. Total references: " + vbaProject.References.Count);
            
            workbook.Save("VbaProjectWithControlReference.xlsm");
        }
    }
}
```

### Ver también

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


