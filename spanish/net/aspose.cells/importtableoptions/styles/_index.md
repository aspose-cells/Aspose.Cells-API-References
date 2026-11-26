---
title: "ImportTableOptions.Styles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Obtiene y establece los estilos para cada columna de la tabla"
type: docs
url: /es/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

Obtiene y establece los estilos para cada columna de la tabla.

```csharp
public Style[] Styles { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyStylesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear tabla de datos de ejemplo
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // Crear ImportTableOptions y establecer la propiedad Styles
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // Crear estilos para cada columna
                Style[] columnStyles = new Style[2];

                // Estilo para la columna Producto (negrita, fuente azul)
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // Estilo para la columna Precio (formato de moneda, fuente verde)
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // Establecer la propiedad Styles
                options.Styles = columnStyles;

                // Importar datos con estilos
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // Mostrar los estilos aplicados
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // Guarda el libro de trabajo
                workbook.Save("StylesDemo.xlsx");
                Console.WriteLine("Workbook saved with styled data.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


