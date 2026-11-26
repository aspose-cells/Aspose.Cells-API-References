---
title: "WorksheetCollection.TableStyles"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Obtiene el objeto TableStyles"
type: docs
url: /es/net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

Obtiene el objeto `TableStyles`.

```csharp
public TableStyleCollection TableStyles { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyTableStylesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunas hojas de cálculo
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            // Crear y agregar estilos de tabla
            int styleIndex1 = workbook.Worksheets.TableStyles.AddTableStyle("Style1");
            TableStyle style1 = workbook.Worksheets.TableStyles[styleIndex1];
            
            int styleIndex2 = workbook.Worksheets.TableStyles.AddTableStyle("Style2");
            TableStyle style2 = workbook.Worksheets.TableStyles[styleIndex2];
            
            // Mostrar el recuento de estilos de tabla
            Console.WriteLine("Table styles count: " + workbook.Worksheets.TableStyles.Count);
            
            // Eliminar un estilo
            workbook.Worksheets.TableStyles.RemoveAt(0);
            
            // Mostrar recuento actualizado
            Console.WriteLine("Table styles count after removal: " + workbook.Worksheets.TableStyles.Count);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


