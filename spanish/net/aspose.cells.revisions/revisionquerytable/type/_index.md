---
title: "RevisionQueryTable.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionQueryTable. Representa el tipo de la revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

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

    public class RevisionQueryTablePropertyTypeDemo
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

                // Crear un RevisionQueryTable simulado (esto es conceptual - en realidad lo obtendrías de revisiones)
                // Dado que no podemos instanciar directamente RevisionQueryTable, demostraremos el patrón
                RevisionQueryTable revisionQueryTable = null;

                // Verificar si tenemos una tabla de consulta de revisión
                if (revisionQueryTable != null)
                {
                    // Mostrar el valor de la propiedad Type (solo lectura)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // Mostrar el valor del enum como entero para referencia
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // Mostrar otras propiedades para contexto
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // Guarda el libro de trabajo
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


