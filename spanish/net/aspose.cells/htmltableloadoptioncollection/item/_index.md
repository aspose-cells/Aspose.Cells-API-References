---
title: "HtmlTableLoadOptionCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlTableLoadOptionCollection. Obtiene el elemento HtmlTableLoadOption en el índice especificado"
type: docs
url: /es/net/aspose.cells/htmltableloadoptioncollection/item/
---
## HtmlTableLoadOptionCollection indexer

Obtiene el elemento [`HtmlTableLoadOption`](../../htmltableloadoption/) en el índice especificado.

```csharp
public HtmlTableLoadOption this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Agregar una nueva HtmlTableLoadOption por índice de tabla
            int index1 = tableLoadOptions.Add(0);

            // Acceder al HtmlTableLoadOption usando la propiedad Item
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Configurar la opción de carga de tabla
            option.TableToListObject = true;
            option.TargetSheetIndex = 1;

            // Cargar archivo HTML con las opciones configuradas
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


