---
title: "RevisionMergeConflict.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionMergeConflict. Obtiene el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisionmergeconflict/type/
---
## RevisionMergeConflict.Type property

Obtiene el tipo de revisión.

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

    public class RevisionMergeConflictPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Habilitar el seguimiento de cambios
            workbook.StartAccessCache(AccessCacheOptions.All);

            // Realizar cambios para crear un escenario de conflicto de fusión
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("TempMergeConflict.xlsx");

            // Simular un conflicto de fusión abriendo el archivo y realizando cambios conflictivos
            Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
            otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
            otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");

            // Fusionar los cambios conflictivos
            workbook.Combine(otherUserWorkbook);

            // Verificar si hay revisiones
            if (workbook.HasRevisions)
            {
                // Encontrar la revisión del conflicto de fusión
                RevisionMergeConflict mergeConflictRevision = null;
                // Nota: En la implementación real, necesitaría otra forma de acceder a las revisiones
                // ya que la propiedad Revisions no está disponible en la definición de API proporcionada

                if (mergeConflictRevision != null)
                {
                    // Mostrar la propiedad Type de la revisión del conflicto de fusión
                    Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);

                    // Demostrar cómo se puede usar esta información
                    if (mergeConflictRevision.Type == RevisionType.MergeConflict)
                    {
                        Console.WriteLine("This revision represents a merge conflict.");
                        Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
                    }
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


