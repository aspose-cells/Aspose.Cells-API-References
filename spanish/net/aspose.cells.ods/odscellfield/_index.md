---
title: "Clase OdsCellField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Ods.OdsCellField. Representa el campo de celda de ods"
type: docs
url: /es/net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

Representa el campo de celda de ODS.

```csharp
public class OdsCellField
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | Obtiene y establece el índice de columna de la celda. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | Representa el formato personalizado del valor del campo. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | Obtiene y establece el tipo del campo. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | Obtiene y establece el índice de fila de la celda. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. Crea un OdsCellField a través de la colección (sin constructor sin parámetros)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // Recupera el campo que acabamos de agregar
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // Escribe algo en la celda identificada por el OdsCellField
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. Agrega el mismo campo nuevamente para demostrar el uso de la colección (opcional)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // Actualiza todos los campos ODS para que se reflejen en el archivo guardado
                odsFields.UpdateFieldsValue();

                // Muestra los valores de las propiedades en la consola
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // Guarda el libro de trabajo como un archivo ODS
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


