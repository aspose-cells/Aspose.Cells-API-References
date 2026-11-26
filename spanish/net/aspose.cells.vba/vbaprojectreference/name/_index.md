---
title: "VbaProjectReference.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProjectReference. Obtiene y establece el nombre de la referencia"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

Obtiene y establece el nombre de la referencia.

```csharp
public string Name { get; set; }
```

### Ejemplos

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
            // Crear un libro de trabajo (el proyecto VBA se crea automáticamente para archivos .xlsm)
            Workbook workbook = new Workbook(FileFormatType.Xlsm);
            
            // Agregar una referencia al proyecto VBA
            string referenceName = "MyReference";
            string referencePath = @"C:\Temp\MyLibrary.dll";
            workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);

            // Acceder y verificar la referencia mediante la propiedad Name
            VbaProjectReferenceCollection references = workbook.VbaProject.References;
            for (int i = 0; i < references.Count; i++)
            {
                if (references[i].Name.Equals(referenceName))
                {
                    Console.WriteLine($"Found reference: {references[i].Name}");
                    break;
                }
            }

            // Guarda el libro de trabajo
            workbook.Save("VbaProjectReferenceDemo.xlsm");
        }
    }
}
```

### Ver también

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


