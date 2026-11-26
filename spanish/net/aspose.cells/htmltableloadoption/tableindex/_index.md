---
title: "HtmlTableLoadOption.TableIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlTableLoadOption. Obtenga o establezca el índice de la tabla a importar desde html"
type: docs
url: /es/net/aspose.cells/htmltableloadoption/tableindex/
---
## HtmlTableLoadOption.TableIndex property

Obtener o establecer el índice de la tabla a importar desde html.

```csharp
public int TableIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();

            // Crear opciones de carga HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Configure la opción de carga de tabla con TableIndex = 0 (primera tabla)
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };

            // Agregue la opción de carga de tabla
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Cargue el archivo HTML (reemplácelo con la ruta real)
            workbook = new Workbook("input.html", loadOptions);

            // Guardar como archivo Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


