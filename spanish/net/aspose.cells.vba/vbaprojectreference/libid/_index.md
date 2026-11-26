---
title: "VbaProjectReference.Libid"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProjectReference. Obtiene y establece el Libid de la referencia"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

Obtiene y establece el Libid de la referencia.

```csharp
public string Libid { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyLibidDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook targetWorkbook = new Workbook();
            
            // Cargar el libro de trabajo fuente con proyecto VBA
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            
            // Eliminar referencias existentes en el destino
            targetWorkbook.VbaProject.References.Clear();
            
            // Copiar referencias del origen al destino
            foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
            {
                if (reference.Type == VbaProjectReferenceType.Registered)
                {
                    // Demostrar el uso de la propiedad Libid
                    targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
                }
                else if (reference.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        reference.Name, 
                        reference.Libid, 
                        reference.Twiddledlibid, 
                        reference.ExtendedLibid);
                }
            }
            
            // Guardar el resultado
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### Ver también

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


