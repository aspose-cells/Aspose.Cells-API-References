---
title: "VbaProjectReference.ExtendedLibid"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProjectReference. Obtiene y establece el Libid extendido de la referencia"
type: docs
url: /es/net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Obtiene y establece el Libid extendido de la referencia.

```csharp
public string ExtendedLibid { get; set; }
```

### Observaciones

Solo para referencia de control.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Inicializar proyecto VBA
                VbaProject vbaProject = workbook.VbaProject;

                // Agregar una referencia de control para demostrar ExtendedLibid
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // Obtener la primera referencia
                VbaProjectReference reference = vbaProject.References[0];

                // Mostrar el valor de la propiedad ExtendedLibid
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // Demostrar la configuración de ExtendedLibid (ya que es de lectura/escritura)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // Guarda el libro de trabajo
                workbook.Save("ExtendedLibidDemo.xlsm");
                Console.WriteLine("Workbook saved successfully with ExtendedLibid demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


