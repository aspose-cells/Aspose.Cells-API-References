---
title: "Clase HtmlTableLoadOption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.HtmlTableLoadOption. Representa la opción al importar una tabla desde HTML"
type: docs
url: /es/net/aspose.cells/htmltableloadoption/
---
## HtmlTableLoadOption class

Representa la opción al importar una tabla desde HTML.

```csharp
public class HtmlTableLoadOption
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HtmlTableLoadOption](htmltableloadoption/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Id](../../aspose.cells/htmltableloadoption/id/) { get; set; } | Obtener o establecer el id de la tabla a importar desde html |
| [Name](../../aspose.cells/htmltableloadoption/name/) { get; set; } | (**Obsoleto.**) Obtener o establecer el nombre de la tabla a importar desde html |
| [OriginalSheetIndex](../../aspose.cells/htmltableloadoption/originalsheetindex/) { get; set; } | Obtener o establecer el índice original de la hoja de cálculo en el html. |
| [TableIndex](../../aspose.cells/htmltableloadoption/tableindex/) { get; set; } | Obtener o establecer el índice de la tabla a importar desde html. |
| [TableToListObject](../../aspose.cells/htmltableloadoption/tabletolistobject/) { get; set; } | Indica si se generan objetos de lista a partir de la tabla importada. El valor predeterminado es false. |
| [TargetSheetIndex](../../aspose.cells/htmltableloadoption/targetsheetindex/) { get; set; } | Obtener o establecer el índice de destino de la hoja de cálculo donde se ubicará la tabla. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionDemo
    {
        public static void HtmlTableLoadOptionExample()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();

            // Crea una instancia de HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Crear una instancia de HtmlTableLoadOption
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                Id = "table1",
                Name = "SampleTable",
                OriginalSheetIndex = 0,
                TargetSheetIndex = 0,
                TableToListObject = true
            };

            // Agregar el HtmlTableLoadOption a los HtmlLoadOptions
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Cargar el archivo HTML en el libro de trabajo con las opciones de carga especificadas
            workbook = new Workbook("HtmlTableLoadOptionExample_original.html", loadOptions);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("HtmlTableLoadOptionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


