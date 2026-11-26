---
title: "TableStyleCollection.GetBuiltinTableStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "TableStyleCollection method. Obtiene el estilo de tabla incorporado"
type: docs
url: /es/net/aspose.cells.tables/tablestylecollection/getbuiltintablestyle/
---
## TableStyleCollection.GetBuiltinTableStyle method

Obtiene el estilo de tabla incorporado

```csharp
public TableStyle GetBuiltinTableStyle(TableStyleType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | TableStyleType | El tipo de estilo de tabla incorporado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleCollectionMethodGetBuiltinTableStyleWithTableStyleTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear una tabla
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Obtener la colección de estilos de tabla
                TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

                // Llamar a GetBuiltinTableStyle con el parámetro TableStyleType
                TableStyle builtinStyle = tableStyles.GetBuiltinTableStyle(TableStyleType.TableStyleMedium2);

                // Aplicar el estilo incorporado a nuestra tabla
                table.TableStyleName = builtinStyle.Name;

                Console.WriteLine($"Applied built-in table style: {builtinStyle.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBuiltinTableStyle method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("TableStyleCollectionMethodGetBuiltinTableStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TableStyle](../../tablestyle/)
* enum [TableStyleType](../../tablestyletype/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


