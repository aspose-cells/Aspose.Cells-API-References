---
title: "ImportTableOptions.ConvertNumericData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ImportTableOptions property. Obtiene o establece un valor que indica si el valor de cadena debe convertirse a numérico o a fecha"
type: docs
url: /es/net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Obtiene o establece un valor que indica si el valor de cadena debe convertirse a numérico o a fecha.

```csharp
public bool ConvertNumericData { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear una tabla de datos de ejemplo con valores numéricos y de cadena
            DataTable dt = new DataTable();
            dt.Columns.Add("Numbers");
            dt.Columns.Add("Text");
            dt.Rows.Add("123", "456");
            dt.Rows.Add("ABC", "DEF");

            // Obtener las celdas de la primera hoja de cálculo
            Cells cells = workbook.Worksheets[0].Cells;

            // Crear opciones de importación con ConvertNumericData establecido en true
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertNumericData = true;
            options.IsFieldNameShown = true;

            // Importar datos con conversión numérica
            cells.ImportData(dt, 0, 0, options);

            // Mostrar resultados
            Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
            Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


