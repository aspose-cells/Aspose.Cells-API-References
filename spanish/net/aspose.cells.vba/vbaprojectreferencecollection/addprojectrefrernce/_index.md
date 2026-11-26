---
title: "VbaProjectReferenceCollection.AddProjectRefrernce"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaProjectReferenceCollection. Añade una referencia a un proyecto VBA externo"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Agrega una referencia a un proyecto VBA externo.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la referencia. |
| absoluteLibid | String | El identificador del proyecto VBA referenciado con una ruta absoluta. |
| relativeLibid | String | El identificador del proyecto VBA referenciado con una ruta relativa. |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método VbaProjectReferenceCollection.AddProjectReferernce(). Este método será eliminado 12 meses después desde julio de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddProjectRefrernceWithStringStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Inicializar proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Añadir una referencia de proyecto con libids absolutos y relativos
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Mostrar el recuento de referencias
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // Guarda el libro de trabajo
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### Ver también

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


