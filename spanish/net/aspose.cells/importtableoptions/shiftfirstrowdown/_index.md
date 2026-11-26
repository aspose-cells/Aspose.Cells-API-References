---
title: "ImportTableOptions.ShiftFirstRowDown"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Indica si se desplaza la primera fila hacia abajo al insertar filas."
type: docs
url: /es/net/aspose.cells/importtableoptions/shiftfirstrowdown/
---
## ImportTableOptions.ShiftFirstRowDown property

Indica si se desplaza la primera fila hacia abajo al insertar filas.

```csharp
public bool ShiftFirstRowDown { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyShiftFirstRowDownDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Crear DataTable de ejemplo
            DataTable table = new DataTable();
            table.Columns.Add("Column1");
            table.Columns.Add("Column2");
            table.Rows.Add("Header1", "Header2");
            table.Rows.Add("Data1", "Data2");
            table.Rows.Add("Data3", "Data4");

            // Importar con ShiftFirstRowDown = false (comportamiento predeterminado).
            var options1 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = false
            };
            cells.ImportData(table, 0, 0, options1);
            Console.WriteLine("With ShiftFirstRowDown=false, first row starts at A1: " + cells[0, 0].StringValue);

            // Borrar la hoja de cálculo e importar con ShiftFirstRowDown = true.
            workbook.Worksheets[0].Cells.Clear();
            var options2 = new ImportTableOptions
            {
                IsFieldNameShown = false,
                ShiftFirstRowDown = true
            };
            cells.ImportData(table, 0, 0, options2);
            Console.WriteLine("With ShiftFirstRowDown=true, first row is shifted down to A2: " + cells[1, 0].StringValue);

            // Guarda el libro de trabajo
            workbook.Save("ShiftFirstRowDownDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


