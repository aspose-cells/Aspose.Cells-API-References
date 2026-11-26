---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TableStyleCollection. Obtiene y establece el nombre del estilo predeterminado de la tabla"
type: docs
url: /es/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

Obtiene y establece el nombre del estilo predeterminado de la tabla.

```csharp
public string DefaultTableStyleName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la colección de estilos de tabla
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Mostrar el nombre del estilo de tabla predeterminado
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Cambia el estilo de tabla predeterminado
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


