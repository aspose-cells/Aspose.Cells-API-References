---
title: "WorkbookSettings.MaxRowsOfSharedFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene y establece el número máximo de filas de la fórmula compartida"
type: docs
url: /es/net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

Obtiene y establece el número máximo de fila de la fórmula compartida.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### Observaciones

Si el número es demasiado grande, el autofiltro funciona muy lento en MS Excel 2013.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowsOfSharedFormulaDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            book.Settings.MaxRowsOfSharedFormula = 100;
            
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Establecer fórmula compartida con 101 filas (excede MaxRowsOfSharedFormula)
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            // Verificar la fórmula en la última celda
            Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
            
            // Incrementar MaxRowsOfSharedFormula y probar de nuevo en una hoja nueva
            book.Settings.MaxRowsOfSharedFormula = 1024;
            Worksheet sheet2 = book.Worksheets.Add("Sheet2");
            cells = sheet2.Cells;
            cells["B1"].SetSharedFormula("=A1", 101, 1);
            
            Console.WriteLine("Formula in B101 (Sheet2): " + cells["B101"].Formula);
            
            book.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


