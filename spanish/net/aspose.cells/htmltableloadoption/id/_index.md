---
title: "HtmlTableLoadOption.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlTableLoadOption. Obtenga o establezca el id de la tabla a importar desde HTML"
type: docs
url: /es/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

Obtener o establecer el id de la tabla a importar desde html

```csharp
public string Id { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Configurar opciones de carga de tabla
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // Agregar opciones de carga de tabla
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Cargar archivo HTML con opciones especificadas
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


