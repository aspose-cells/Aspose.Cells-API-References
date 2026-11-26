---
title: "RevisionInsertSheet.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionInsertSheet. Obtiene el nombre de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Obtiene el nombre de la hoja de cálculo.

```csharp
public string Name { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo para potencialmente generar un registro de revisión
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // Simular el acceso a un RevisionInsertSheet desde revisiones
                // Nota: En un escenario real, esto provendría de workbook.Revisions
                // Para la demostración, crearemos un escenario simulado
                RevisionInsertSheet insertSheetRevision = null;

                // En el uso real, obtendrías esto de la colección de revisiones
                // Por ejemplo: insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // Dado que no podemos crear RevisionInsertSheet directamente, lo demostraremos
                // lo que harías si tuvieras acceso a uno
                if (insertSheetRevision != null)
                {
                    // Mostrar el valor de la propiedad Name (solo lectura)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // Demostrar el uso de la propiedad Name en una condición
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // Guarda el libro de trabajo
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


