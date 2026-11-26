---
title: "RevisionQueryTable.CellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionQueryTable. Obtiene la ubicación de la tabla de consulta afectada"
type: docs
url: /es/net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

Obtiene la ubicación de la tabla de consulta afectada.

```csharp
public CellArea CellArea { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyCellAreaDemo
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
                // En un escenario real, obtendrías revisiones del libro de trabajo
                // Para demostración, crearemos un ejemplo conceptual
                // Nota: las instancias de RevisionQueryTable se obtienen típicamente de las revisiones del libro de trabajo
                RevisionQueryTable revisionQueryTable = null;

                // Verificar si tenemos una tabla de consulta de revisión
                if (revisionQueryTable != null)
                {
                    // Mostrar el valor de la propiedad CellArea (solo lectura)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // Mostrar otras propiedades para contexto
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // Guarda el libro de trabajo
                workbook.Save("CellAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


