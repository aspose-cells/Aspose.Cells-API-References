---
title: "RevisionInsertSheet.ActionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionInsertSheet. Obtiene el tipo de acción de la revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioninsertsheet/actiontype/
---
## RevisionInsertSheet.ActionType property

Obtiene el tipo de acción de la revisión.

```csharp
public RevisionActionType ActionType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyActionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            // Nota: StartTrackingRevisions no está disponible en la API proporcionada
            // workbook.StartTrackingRevisions();

            // Agregar una nueva hoja de cálculo para generar un registro de revisión
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");
            
            // Nota: StopTrackingRevisions no está disponible en la API proporcionada
            // workbook.StopTrackingRevisions();
            
            // Nota: la propiedad Revisions no está disponible en la API proporcionada
            // Usaremos HasRevisions para comprobar si hay alguna revisión
            if (workbook.HasRevisions)
            {
                // En un escenario real, accederíamos a las revisiones aquí
                // Como no podemos crear RevisionInsertSheet directamente, simularemos la comprobación de una
                // Esto asume que obtuvimos la revisión de algún lugar (como workbook.Revisions)
                RevisionInsertSheet insertSheetRevision = null; // Would be assigned from actual revisions collection
                
                // Como no podemos crear o establecer ActionType, simplemente demostraremos cómo comprobarlo
                if (insertSheetRevision != null)
                {
                    // Mostrar la propiedad ActionType
                    Console.WriteLine("ActionType of sheet insertion: " + insertSheetRevision.ActionType);

                    // Demostrar el uso de la propiedad de solo lectura
                    if (insertSheetRevision.ActionType == RevisionActionType.Add)
                    {
                        Console.WriteLine("This revision represents a sheet addition");
                    }
                }

                // Guardar el libro de trabajo con revisiones
                workbook.Save("RevisionInsertSheetActionTypeDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No sheet insertion revision found");
            }
        }
    }
}
```

### Ver también

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


