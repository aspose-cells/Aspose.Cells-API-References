---
title: "Cell.IsCheckBoxStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si esta celda se establece como casilla de verificación"
type: docs
url: /es/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Indica si se establece esta celda como una casilla de verificación.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda a la celda B1 y configúrela con estilo de casilla de verificación
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // Acceda a la celda A1 y configúrela con estilo de casilla de verificación con un valor
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // Guarda el libro de trabajo
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // Cargue el libro de trabajo guardado para verificar las propiedades
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // Verifique que B1 tenga estilo de casilla de verificación
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // Cambie B1 a estilo sin casilla de verificación y guarde
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


