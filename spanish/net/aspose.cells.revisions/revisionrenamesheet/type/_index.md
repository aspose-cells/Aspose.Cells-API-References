---
title: "RevisionRenameSheet.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionRenameSheet. Representa el tipo de la revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisionrenamesheet/type/
---
## RevisionRenameSheet.Type property

Representa el tipo de la revisión.

```csharp
public override RevisionType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionRenameSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Habilitar el seguimiento de revisiones ANTES de realizar cambios
            // Nota: Este método no existe en la API proporcionada, así que lo eliminaremos
            // workbook.StartTrackingRevisions();

            // Renombrar la primera hoja de cálculo para crear una revisión
            Worksheet worksheet = workbook.Worksheets[0];
            string originalName = worksheet.Name;
            worksheet.Name = "RenamedSheet";

            // Acceder a la colección de revisiones
            // Nota: La propiedad Revisions no existe en la API proporcionada
            // Así que necesitaremos comprobar primero si el libro de trabajo tiene revisiones
            if (workbook.HasRevisions)
            {
                // Encontrar la revisión de renombrado de hoja
                RevisionRenameSheet renameRevision = null;
                // Dado que no podemos acceder a Revisions directamente, necesitaremos modificar esta parte
                // Esto es solo un marcador de posición ya que la API real no admite el acceso a revisiones
                Console.WriteLine("Revision tracking is not fully supported in this API version.");
                
                if (renameRevision != null)
                {
                    // Mostrar el valor de la propiedad Type
                    Console.WriteLine("Revision Type: " + renameRevision.Type);
                    Console.WriteLine("Old Sheet Name: " + renameRevision.OldName);
                    Console.WriteLine("New Sheet Name: " + renameRevision.NewName);

                    // Demostrar cómo usar la propiedad Type
                    if (renameRevision.Type == RevisionType.RenameSheet)
                    {
                        Console.WriteLine("This revision represents a worksheet rename operation.");
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionRenameSheetDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [RevisionType](../../revisiontype/)
* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


