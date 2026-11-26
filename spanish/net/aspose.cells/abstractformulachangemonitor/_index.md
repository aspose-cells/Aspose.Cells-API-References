---
title: "Clase AbstractFormulaChangeMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AbstractFormulaChangeMonitor. Monitor para que el usuario siga el cambio de fórmulas durante ciertas operaciones"
type: docs
url: /es/net/aspose.cells/abstractformulachangemonitor/
---
## AbstractFormulaChangeMonitor class

Monitorea para que el usuario siga el cambio de fórmulas durante ciertas operaciones.

```csharp
public abstract class AbstractFormulaChangeMonitor
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [OnCellFormulaChanged](../../aspose.cells/abstractformulachangemonitor/oncellformulachanged/)(int, int, int) | El evento que se activará cuando la fórmula en una celda cambie. |
| virtual [OnFormatConditionFormulaChanged](../../aspose.cells/abstractformulachangemonitor/onformatconditionformulachanged/)(FormatCondition) | El evento que se activará cuando la fórmula de FormatCondition cambie. |

### Observaciones

Por ejemplo, al eliminar/insertar un rango de celdas, las fórmulas de otras celdas pueden cambiar debido al desplazamiento de referencias. Tenga en cuenta que los métodos en el monitor pueden invocarse varias veces para un mismo objeto que contiene la fórmula.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassAbstractFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Establece algunas fórmulas en celdas
            worksheet.Cells["A1"].Formula = "=B1+C1";
            worksheet.Cells["B1"].Formula = "=D1*2";
            worksheet.Cells["C1"].Value = 5;
            worksheet.Cells["D1"].Value = 10;

            InsertOptions options = new InsertOptions();
            options.FormulaChangeMonitor = new MyFormulaChangeMonitor(wb.Worksheets);
            
            // Inserta filas que desencadenarán cambios de fórmula
            worksheet.Cells.InsertRows(0, 2, options);
        }
    }

    public class MyFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        private readonly WorksheetCollection mWorksheets;
        
        public MyFormulaChangeMonitor(WorksheetCollection worksheets)
        {
            mWorksheets = worksheets;
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            Console.WriteLine($"Formula changed in {mWorksheets[sheetIndex].Name}!{CellsHelper.CellIndexToName(rowIndex, columnIndex)}");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


