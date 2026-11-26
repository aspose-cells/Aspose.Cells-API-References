---
title: "WorksheetCollection.ActiveSheetName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/activesheetname/
---
## WorksheetCollection.ActiveSheetName property

Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo.

```csharp
public string ActiveSheetName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyActiveSheetNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunas hojas de cálculo
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Establecer la hoja activa por nombre
            workbook.Worksheets.ActiveSheetName = "Sheet2";

            // Verificar la hoja activa
            Console.WriteLine("Active Sheet: " + workbook.Worksheets.ActiveSheetName);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


