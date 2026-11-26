---
title: "Enumeración AutoFitMergedCellsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.AutoFitMergedCellsType. Representa el tipo de ajuste automático de celdas combinadas"
type: docs
url: /es/net/aspose.cells/autofitmergedcellstype/
---
## AutoFitMergedCellsType enumeration

Representa el tipo de ajuste automático de celdas combinadas.

```csharp
public enum AutoFitMergedCellsType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Ignorar celdas combinadas. |
| FirstLine | `1` | Solo expande la altura de la primera fila. |
| LastLine | `2` | Solo expande la altura de la última fila. |
| EachLine | `3` | Expande la altura de cada fila. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitMergedCellsTypeDemo
    {
        public static void AutoFitMergedCellsTypeExample()
        {
            //Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            //Obteniendo la referencia de la hoja de cálculo recién añadida
            Worksheet sheet1 = workbook.Worksheets[0];

            // Crear un rango A1:B2
            Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);

            // Combina las celdas
            range.Merge();

            // Insertar valor en la celda combinada A1
            sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Cree un objeto de estilo
            Style style = sheet1.Cells[0, 0].GetStyle();

            // Activar ajuste de texto
            style.IsTextWrapped = true;

            // Aplique el estilo a la celda
            sheet1.Cells[0, 0].SetStyle(style);

            // Crear un objeto para AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions();

            // Solo expande la altura de la primera fila.
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;

            // Ajustar automáticamente filas en la hoja (incluyendo las celdas combinadas)
            sheet1.AutoFitRows(options);


            int index = workbook.Worksheets.Add();
            Worksheet sheet2 = workbook.Worksheets[index];
            sheet2.Name = "Sheet2";
            // Crear un rango A1:B2
            Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);

            // Combina las celdas
            range2.Merge();

            // Insertar valor en la celda combinada A1
            sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Cree un objeto de estilo
            Style style2 = sheet2.Cells[0, 0].GetStyle();

            // Activar ajuste de texto
            style2.IsTextWrapped = true;

            // Aplique el estilo a la celda
            sheet2.Cells[0, 0].SetStyle(style);

            // Crear un objeto para AutoFitterOptions
            AutoFitterOptions options2 = new AutoFitterOptions();

            // Solo expande la altura de la última fila.
            options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;

            // Ajustar automáticamente filas en la hoja (incluyendo las celdas combinadas)
            sheet2.AutoFitRows(options2);


            index = workbook.Worksheets.Add();
            Worksheet sheet3 = workbook.Worksheets[index];
            sheet3.Name = "Sheet3";
            // Crear un rango A1:B2
            Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);

            // Combina las celdas
            range3.Merge();

            // Insertar valor en la celda combinada A1
            sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Cree un objeto de estilo
            Style style3 = sheet3.Cells[0, 0].GetStyle();

            // Activar ajuste de texto
            style3.IsTextWrapped = true;

            // Aplique el estilo a la celda
            sheet3.Cells[0, 0].SetStyle(style);

            // Crear un objeto para AutoFitterOptions
            AutoFitterOptions options3 = new AutoFitterOptions();

            // Solo expande la altura de cada fila.
            options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;

            // Ajustar automáticamente filas en la hoja (incluyendo las celdas combinadas)
            sheet3.AutoFitRows(options3);


            index = workbook.Worksheets.Add();
            Worksheet sheet4 = workbook.Worksheets[index];
            sheet4.Name = "Sheet4";
            // Crear un rango A1:B2
            Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);

            // Combina las celdas
            range4.Merge();

            // Insertar valor en la celda combinada A1
            sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // Cree un objeto de estilo
            Style style4 = sheet4.Cells[0, 0].GetStyle();

            // Activar ajuste de texto
            style4.IsTextWrapped = true;

            // Aplique el estilo a la celda
            sheet4.Cells[0, 0].SetStyle(style);

            // Crear un objeto para AutoFitterOptions
            AutoFitterOptions options4 = new AutoFitterOptions();

            // Ignorar celdas combinadas.
            options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;

            // Ajustar automáticamente filas en la hoja (sin incluir las celdas combinadas)
            sheet4.AutoFitRows(options4);

            // Guarda el libro de trabajo
            workbook.Save("AutoFitMergedCellsTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


