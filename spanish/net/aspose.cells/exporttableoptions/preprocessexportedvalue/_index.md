---
title: "ExportTableOptions.PreprocessExportedValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ExportTableOptions. Preprocesar el valor de la celda actual que se exportará"
type: docs
url: /es/net/aspose.cells/exporttableoptions/preprocessexportedvalue/
---
## ExportTableOptions.PreprocessExportedValue method

Preprocesa el valor de la celda actual para exportarlo.

```csharp
public virtual bool PreprocessExportedValue(int cellRow, int cellColumn, CellValue value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellRow | Int32 | el índice de fila de la celda actual |
| cellColumn | Int32 | el índice de columna de la celda |
| valor | CellValue | valor y tipo de la celda actual |

### Valor de retorno

Si la celda actual ha sido reemplazada con un tipo y/o valor diferente.

### Observaciones

El índice de fila y columna es el índice absoluto de la celda en la hoja de cálculo, no el índice en la tabla exportada. El usuario puede comprobar el valor de la celda actual en la implementación sobrescrita de este método; si la celda actual necesita ser reemplazada por otro tipo y valor, aquí la implementación debe establecer el tipo y valor esperados en el objeto CellValue y devolver true. Por defecto, este método no hace nada y devuelve false.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExportTableOptionsMethodPreprocessExportedValueWithInt32Int32CellValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells["A2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(DateTime.Now);

            // Cree una instancia de ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions();

            // Crear un objeto CellValue para demostración
            CellValue cellValue = new CellValue();
            cellValue.Type = CellValueType.IsString;
            cellValue.Value = "Processed Value";

            try
            {
                // Llamar a PreprocessExportedValue con parámetros específicos (fila 0, columna 0, CellValue)
                bool result = exportOptions.PreprocessExportedValue(0, 0, cellValue);

                // Mostrar el resultado de la llamada al método
                Console.WriteLine($"PreprocessExportedValue returned: {result}");

                // Modificar la celda con el valor procesado si es necesario
                if (result)
                {
                    worksheet.Cells[0, 0].PutValue(cellValue.Value);
                }

                // Guarda el libro de trabajo
                workbook.Save("PreprocessExportedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PreprocessExportedValue method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellValue](../../cellvalue/)
* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


