---
title: "Cells.OdsCellFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene la lista de campos de ods"
type: docs
url: /es/net/aspose.cells/cells/odscellfields/
---
## Cells.OdsCellFields property

Obtiene la lista de campos de ods.

```csharp
public OdsCellFieldCollection OdsCellFields { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsPropertyOdsCellFieldsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección Cells
            Cells cells = worksheet.Cells;

            try
            {
                // Acceder a la propiedad OdsCellFields (solo lectura)
                var odsCellFields = cells.OdsCellFields;

                // Mostrar información sobre la colección OdsCellFields
                Console.WriteLine("OdsCellFields collection count: " + odsCellFields.Count);

                // Iterar a través de la colección OdsCellFields
                for (int i = 0; i < odsCellFields.Count; i++)
                {
                    var field = odsCellFields[i];
                    Console.WriteLine($"Field {i}: Type - {field.FieldType}");
                }

                // Demostrar la actualización de valores de campos
                odsCellFields.UpdateFieldsValue();

                Console.WriteLine("OdsCellFields demonstration completed successfully.");
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

* class [OdsCellFieldCollection](../../../aspose.cells.ods/odscellfieldcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


