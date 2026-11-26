---
title: "Column.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Column. Obtiene el estilo de esta columna"
type: docs
url: /es/net/aspose.cells/column/style/
---
## Column.Style property

Obtiene el estilo de esta columna.

```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Column.GetStyle() para obtener el estilo predeterminado de esta columna. Esta propiedad será eliminada 12 meses después, a partir de diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la primera columna
            Column column = worksheet.Cells.Columns[0];
            
            // Obtener el estilo actual usando la propiedad Style
            Style originalStyle = column.Style;
            Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
            
            // Crear un nuevo estilo y modificar propiedades
            Style newStyle = workbook.CreateStyle();
            newStyle.BackgroundColor = Color.LightBlue;
            newStyle.Font.IsBold = true;
            newStyle.HorizontalAlignment = TextAlignmentType.Center;
            
            // Aplicar el nuevo estilo a la columna
            column.SetStyle(newStyle);
            
            // Agregar datos para demostrar la aplicación del estilo
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Verificar los cambios de estilo
            Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
            
            // Guardar con ajuste del ancho de columna
            column.Width = 15;
            workbook.Save("ColumnStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


