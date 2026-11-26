---
title: "ExportTableOptions.CheckMixedValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExportTableOptions. False Aspose.Cells establecerá el tipo de DataColumns según el tipo de valor de la primera fila para mejorar el rendimiento. True Aspose.Cells comprobará si el tipo de valor en la columna está mezclado antes de establecer el tipo de DataColumns y, si los tipos de valor están mezclados, el tipo de DataColumns será string."
type: docs
url: /es/net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False, Aspose.Cells establecerá el tipo de DataColumn según el tipo de valor de la primera fila por rendimiento. True, Aspose.Cells comprobará si el tipo de valor en la columna está mezclado antes de establecer el tipo de DataColumn y, si los tipos de valor están mezclados, el tipo de DataColumn será string.

```csharp
public bool CheckMixedValueType { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar encabezados
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value Date");

            // Agregar datos de muestra con tipos mixtos
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue("2023-01-15");
            worksheet.Cells["A4"].PutValue("3");
            worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));

            // Crear opciones de exportación con CheckMixedValueType habilitado
            ExportTableOptions options = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true
            };

            // Exportar datos a DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);

            // Mostrar resultados
            Console.WriteLine("Columns: " + dataTable.Columns.Count);
            Console.WriteLine("Rows: " + dataTable.Rows.Count);
            Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
            Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
        }
    }
}
```

### Ver también

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


