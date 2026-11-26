---
title: "HtmlTableLoadOption.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlTableLoadOption. Obtenga o establezca el nombre de la tabla a importar desde html"
type: docs
url: /es/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

Obtenga o establezca el nombre de la tabla a importar desde html

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();

            // Crear HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Acceda a HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Agregar una nueva HtmlTableLoadOption por índice de tabla
            int index = tableLoadOptions.Add(0);

            // Acceda a HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];

            // Establezca la propiedad Name
            option.Name = "CustomerDataTable";

            // Cargue un archivo HTML (reemplácelo con la ruta real del archivo)
            workbook = new Workbook("input.html", loadOptions);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


