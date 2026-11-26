---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. Obtenga la instancia de HtmlTableLoadOptionCollection"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

Obtén la instancia de HtmlTableLoadOptionCollection

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // Agregar opciones de carga de tabla por índice
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // Agregar opciones de carga de tabla por ID
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Cargue el archivo HTML con las opciones
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Guardar la salida
            workbook.Save("output.xlsx");
            
            // Borrar y agregar nuevas opciones de carga de tabla
            loadOptions.TableLoadOptions.Clear();
            
            // Agregar opciones de carga de tabla con mapeo de índice de hoja
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // Agregar opciones de carga de tabla con ID y mapeo de hoja
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // Cargar y guardar nuevamente con nuevas opciones
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### Ver también

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


