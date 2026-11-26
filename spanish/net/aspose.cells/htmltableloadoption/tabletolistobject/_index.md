---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlTableLoadOption. Indica si se generan objetos de lista a partir de la tabla importada. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

Indica si se generan objetos de lista a partir de la tabla importada. El valor predeterminado es false.

```csharp
public bool TableToListObject { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();

            // Cree opciones de carga HTML con TableToListObject habilitado
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Cargue HTML con las opciones especificadas
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


