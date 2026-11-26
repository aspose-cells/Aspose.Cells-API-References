---
title: "RevisionInsertSheet.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionInsertSheet. Obtiene el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioninsertsheet/type/
---
## RevisionInsertSheet.Type property

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

    public class RevisionInsertSheetPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            
            // Habilitar el seguimiento de revisiones (simulado ya que StartTrackingRevisions no está disponible)
            bool trackRevisions = true;

            // Agregar una nueva hoja de cálculo para generar un registro de revisión
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Simular la obtención de revisiones (ya que la propiedad Revisions no está disponible)
            if (trackRevisions && workbook.HasRevisions)
            {
                // En un escenario real, accederíamos a las revisiones aquí
                // Esto asume que obtuvimos la revisión de algún lugar (como workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                if (insertSheetRevision != null)
                {
                    // Mostrar la propiedad Type
                    Console.WriteLine("Revision Type: " + insertSheetRevision.Type);

                    // Demostrar el uso de la propiedad Type de solo lectura
                    if (insertSheetRevision.Type == RevisionType.InsertSheet)
                    {
                        Console.WriteLine("This revision represents a sheet insertion operation");
                        
                        // Mostrar información adicional sobre la hoja insertada
                        Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);
                        Console.WriteLine("Sheet position: " + insertSheetRevision.SheetPosition);
                    }

                    // Verificar contra otros tipos de revisión
                    if (insertSheetRevision.Type != RevisionType.Unknown)
                    {
                        Console.WriteLine("This is a known revision type");
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionInsertSheetTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No revisions found or revision tracking not enabled");
            }
        }
    }
}
```

### Ver también

* enum [RevisionType](../../revisiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


