---
title: "WorksheetCollection.Dxfs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Obtiene los registros maestros de formato diferencial"
type: docs
url: /es/net/aspose.cells/worksheetcollection/dxfs/
---
## WorksheetCollection.Dxfs property

Obtiene los registros maestros de formato diferencial.

```csharp
public DxfCollection Dxfs { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyDxfsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Establecer condición y estilo
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            fcc[0].Style = style;
            
            // Demostrar la propiedad Dxfs
            Console.WriteLine("Dxfs count before applying formatting: " + workbook.Worksheets.Dxfs.Count);
            
            // Aplicar formato que se añadirá a Dxfs
            worksheet.ConditionalFormattings[0][0].Priority = 1;
            
            Console.WriteLine("Dxfs count after applying formatting: " + workbook.Worksheets.Dxfs.Count);
        }
    }
}
```

### Ver también

* class [DxfCollection](../../dxfcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


