---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TableStyleCollection. Obtiene y establece el nombre del estilo predeterminado de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Obtiene y establece el nombre del estilo predeterminado de la tabla dinámica.

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la colección de estilos de tabla
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Mostrar el nombre del estilo predeterminado de la tabla dinámica
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Cambiar el estilo predeterminado de la tabla dinámica
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // Verificar el cambio
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
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


