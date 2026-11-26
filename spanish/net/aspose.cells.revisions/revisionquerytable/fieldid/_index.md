---
title: "RevisionQueryTable.FieldId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionQueryTable. Obtiene el ID del campo de tabla de consulta específico que fue eliminado"
type: docs
url: /es/net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Obtiene el ID del campo específico de la tabla de consulta que fue eliminado.

```csharp
public int FieldId { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // Crear una tabla de consulta (este es un ejemplo simplificado)
                // Nota: En un escenario real, necesitarías crear una tabla de consulta primero
                // Para propósitos de demostración, simularemos el acceso a un RevisionQueryTable

                // Dado que no podemos crear directamente un RevisionQueryTable en este ejemplo simplificado,
                // demostraremos cómo acceder a la propiedad FieldId si tuviéramos una
                // Esto muestra el patrón para leer la propiedad de solo lectura

                // Simular la obtención de un RevisionQueryTable de revisiones (conceptual)
                // En realidad, obtendrías esto de workbook.Revisions o similar
                RevisionQueryTable revisionQueryTable = null;

                // Verificar si tenemos una tabla de consulta de revisión (esto es solo para demostración)
                if (revisionQueryTable != null)
                {
                    // Mostrar el valor de la propiedad FieldId
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // Mostrar otras propiedades para contexto
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // Guarda el libro de trabajo
                workbook.Save("FieldIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


