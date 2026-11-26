---
title: "OdsCellFieldCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsCellFieldCollection. Obtiene el campo por el índice"
type: docs
url: /es/net/aspose.cells.ods/odscellfieldcollection/item/
---
## OdsCellFieldCollection indexer (1 of 2)

Obtiene el campo por el índice.

```csharp
public OdsCellField this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar campos de celda ODS con parámetro de formato
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "");
            sheet.Cells.OdsCellFields.Add(0, 1, OdsCellFieldType.SheetName, "");

            // Acceder a los campos usando la propiedad Item
            OdsCellField titleField = sheet.Cells.OdsCellFields[0];
            OdsCellField sheetNameField = sheet.Cells.OdsCellFields[1];

            // Mostrar tipos de campo
            Console.WriteLine("Field 0 Type: " + titleField.FieldType);
            Console.WriteLine("Field 1 Type: " + sheetNameField.FieldType);

            // Guardar y recargar
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Verificar los campos persistidos
            Console.WriteLine("Reloaded Field 0 Type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Reloaded Field 1 Type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### Ver también

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)

---

## OdsCellFieldCollection indexer (2 of 2)

Obtiene el campo por el índice de fila y columna.

```csharp
public OdsCellField this[int row, int column] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fila | El índice de fila. |
| columna | El índice de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos campos de celda ODS
            // (fila, columna, tipo de campo, formato)
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "TitleFormat");
            sheet.Cells.OdsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);

            try
            {
                // Acceder a los campos usando la propiedad Item (indexador)
                // 1) Por índice de colección
                OdsCellField firstField = sheet.Cells.OdsCellFields[0];
                Console.WriteLine("First field type (by index): " + firstField.FieldType);

                // 2) Por posición de celda (fila, columna)
                OdsCellField titleField = sheet.Cells.OdsCellFields[0, 0];
                Console.WriteLine("Field at (0,0) type (by position): " + titleField.FieldType);

                // Actualizar las celdas con los valores de los campos
                sheet.Cells.OdsCellFields.UpdateFieldsValue();

                // Guardar el libro (el formato ODS conserva los campos)
                workbook.Save("OdsCellFieldItemDemo.ods");
                Console.WriteLine("Workbook saved as OdsCellFieldItemDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


