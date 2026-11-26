---
title: "PasteOptions.OnlyVisibleCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PasteOptions. True significa copiar solo celdas visibles"
type: docs
url: /es/net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

True indica que solo se copian celdas visibles.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOnlyVisibleCellsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Obtener celdas de la primera hoja de cálculo y rellenar datos
            Cells sourceCells = workbook.Worksheets[0].Cells;
            sourceCells["A1"].PutValue("Hidden A1");
            sourceCells["B2"].PutValue("Visible B2");
            sourceCells["C3"].PutValue("Hidden C3");
            
            // Ocultar algunas filas y columnas
            sourceCells.HideRow(0);  // Hides row 1 (A1)
            sourceCells.HideColumn(2); // Hides column C (C3)

            // Crear rango de origen para copiar
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
            
            // Obtener celdas de la segunda hoja de cálculo para el destino
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            
            // Crear opciones de pegado y establecer OnlyVisibleCells
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            
            // Copiar solo celdas visibles
            destRange.Copy(sourceRange, pasteOptions);
            
            // Mostrar resultados para demostrar la funcionalidad
            Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
            Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
            Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
        }
    }
}
```

### Ver también

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


