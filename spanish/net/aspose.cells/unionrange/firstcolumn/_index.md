---
title: "UnionRange.FirstColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene el índice de la primera columna del rango"
type: docs
url: /es/net/aspose.cells/unionrange/firstcolumn/
---
## UnionRange.FirstColumn property

Obtiene el índice de la primera columna del rango.

```csharp
public int FirstColumn { get; }
```

### Observaciones

Solo tiene efecto cuando solo contiene un rango.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // Crea un rango de unión
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C1");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A2:C2");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Muestra la propiedad FirstColumn
            Console.WriteLine("First column index of the union range: " + unionRange.FirstColumn);

            // Demuestra el uso de FirstColumn en operaciones
            Console.WriteLine("First column name: " + CellsHelper.ColumnIndexToName(unionRange.FirstColumn));

            // Aplica formato a la primera columna del rango de unión
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range firstColumnRange = worksheet.Cells.CreateRange(
                unionRange.FirstRow, unionRange.FirstColumn,
                unionRange.RowCount, 1);
            firstColumnRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Guardar el resultado
            workbook.Save("UnionRangePropertyFirstColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


