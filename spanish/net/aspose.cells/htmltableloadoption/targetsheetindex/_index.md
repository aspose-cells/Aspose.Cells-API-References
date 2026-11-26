---
title: "HtmlTableLoadOption.TargetSheetIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlTableLoadOption. Obtenga o establezca el índice de destino de la hoja de cálculo donde se ubicará la tabla"
type: docs
url: /es/net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

Obtener o establecer el índice de destino de la hoja de cálculo donde se ubicará la tabla.

```csharp
public int TargetSheetIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Configure las opciones de carga de tabla con TargetSheetIndex
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
            
            // Agregar opciones de carga de tabla
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);
            
            // Cargue el archivo HTML con opciones
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verifique que las tablas se hayan cargado en las hojas correctas
            Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
            Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


