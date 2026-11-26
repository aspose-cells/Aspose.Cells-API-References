---
title: "Clase AutoFitterOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AutoFitterOptions. Representa todas las opciones de ajuste automático"
type: docs
url: /es/net/aspose.cells/autofitteroptions/
---
## AutoFitterOptions class

Representa todas las opciones del autoajuste.

```csharp
public class AutoFitterOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) Indica si se ajusta automáticamente la altura de la fila cuando las celdas están fusionadas en una fila. El valor predeterminado es false. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | Obtiene y establece el tipo de ajuste automático de la altura de fila de celdas fusionadas. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | Obtiene y establece el tipo de ajuste automático del texto envuelto. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | Obtiene o establece el idioma de edición predeterminado. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | Obtiene y establece la estrategia de formato. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | Indica si es adecuado para fines de renderizado. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | Ignora las filas/columnas ocultas. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | Obtiene y establece la altura máxima de fila (en unidades de Point) al ajustar automáticamente las filas. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | Indica si solo se ajustan las filas cuya altura no está personalizada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitterOptionsDemo
    {
        public static void AutoFitterOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // Crear un rango A1:B2
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // Combina las celdas
            range.Merge();

            // Crea una instancia de AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // Aplica ajuste automático de filas con las opciones especificadas
            worksheet.AutoFitRows(options);

            // Guarda el libro de trabajo
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


