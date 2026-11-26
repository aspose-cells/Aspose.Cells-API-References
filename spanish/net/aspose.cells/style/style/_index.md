---
title: "Style.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor Style. Inicializa una nueva instancia de la clase Style"
type: docs
url: /es/net/aspose.cells/style/style/
---
## Style constructor

Inicializa una nueva instancia de la clase [`Style`](../).

```csharp
[Obsolete("Use CellsFactory.CreateStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style()
```

### Observaciones

NOTA: Este constructor está ahora obsoleto. En su lugar, utilice el método CellsFactory.CreateStyle(). Esta propiedad será eliminada 6 meses después desde octubre de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree un estilo usando el constructor
            Style style = new Style();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Text");
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("StyleConstructorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


