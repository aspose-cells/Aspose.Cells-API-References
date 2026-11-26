---
title: "ImportTableOptions.IsFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Indica si los datos son fórmulas"
type: docs
url: /es/net/aspose.cells/importtableoptions/isformulas/
---
## ImportTableOptions.IsFormulas property

Indica si los datos son fórmulas.

```csharp
public bool[] IsFormulas { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFormulasDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear tabla de datos de muestra con contenido de fórmula
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1");
            dt.Rows.Add("=SUM(1,2,3)");
            dt.Rows.Add("=AVERAGE(4,5,6)");

            // Establecer opciones de importación con la propiedad IsFormulas
            ImportTableOptions options = new ImportTableOptions();
            options.IsFormulas = new bool[] { true }; // Treat first column as formulas
            
            // Importar datos con fórmulas
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);

            // Verificar que las fórmulas se importaron correctamente
            Console.WriteLine("Cell A1 formula: " + workbook.Worksheets[0].Cells["A1"].Formula);
            Console.WriteLine("Cell A2 formula: " + workbook.Worksheets[0].Cells["A2"].Formula);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


