---
title: "HtmlTableLoadOptionCollection.TableToListObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlTableLoadOptionCollection. Indica si se generan objetos de lista a partir de tablas importadas. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

Indica si generar objetos de lista a partir de tablas importadas. El valor predeterminado es false.

```csharp
public bool TableToListObject { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();

            // Crear HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Acceder a la instancia de HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Establezca la propiedad TableToListObject para convertir tablas HTML en ListObjects
            tableLoadOptions.TableToListObject = true;

            // Agregue una tabla para convertirla en ListObject por índice
            tableLoadOptions.Add(0);

            // Cargar un archivo HTML en el libro de trabajo usando las opciones de carga
            workbook = new Workbook("input.html", loadOptions);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


