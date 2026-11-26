---
title: "Clase ExportTableOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ExportTableOptions. Representa todas las opciones de exportación de tabla"
type: docs
url: /es/net/aspose.cells/exporttableoptions/
---
## ExportTableOptions class

Representa todas las opciones de exportación de tabla.

```csharp
public class ExportTableOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | Este valor indica si se permiten DBNulls en esta tabla. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False, Aspose.Cells establecerá el tipo de DataColumn según el tipo de valor de la primera fila por rendimiento. True, Aspose.Cells comprobará si el tipo de valor en la columna está mezclado antes de establecer el tipo de DataColumn y, si los tipos de valor están mezclados, el tipo de DataColumn será string. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | Obtiene y establece el DataTable al que se asigna el tipo de datos de las columnas. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | Exporta el valor de cadena HTML de las celdas al DataTable. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | Exporta el valor de cadena de las celdas al DataTable. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | Indica si los datos de la primera fila se exportan al nombre de columna del DataTable. El valor predeterminado es false. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | Obtiene y establece la estrategia de formato al exportar el valor como cadena. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | Los índices de columnas/filas que deben exportarse. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | True si una fila en el archivo Workbook representa una fila en el DataTable. False si una columna en el archivo Workbook representa una fila en el DataTable. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | Solo exporta celdas visibles. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | Solo exporta columnas visibles. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | Solo exporta filas visibles. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | Estrategia para nombres duplicados de columnas. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | Indica si se omite el valor no válido para la columna. Por ejemplo, si el tipo de columna es decimal, el valor es mayor que decimal.MaxValue y esta propiedad es true, no lanzaremos la excepción nuevamente. El valor predeterminado es false. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | Preprocesa el valor de la celda actual para exportarlo. |

### Observaciones

Si existen requisitos especiales sobre la exportación, como ignorar valores de error, el usuario puede extender esta clase para sobrescribir las APIs correspondientes y lograr el objetivo.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ExportTableOptionsDemo
    {
        public static void ExportTableOptionsExample()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
            worksheet.Cells[2, 1].PutValue(25);

            // Cree una instancia de ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                SkipErrorValue = true,
                PlotVisibleCells = true,
                PlotVisibleRows = true,
                PlotVisibleColumns = true,
                ExportAsString = false,
                ExportAsHtmlString = false,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                CheckMixedValueType = true,
                AllowDBNull = true,
                IsVertical = true,
                RenameStrategy = RenameStrategy.Digit
            };

            // Exporte los datos de la hoja de cálculo a un DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Mostrar los datos exportados
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Guarda el libro de trabajo
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
    }

}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


