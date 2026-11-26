---
title: "DeleteOptions.FormulaChangeMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DeleteOptions. Obtiene/establece el monitor para rastrear los cambios causados por la eliminación"
type: docs
url: /es/net/aspose.cells/deleteoptions/formulachangemonitor/
---
## DeleteOptions.FormulaChangeMonitor property

Obtiene/establece el monitor para rastrear los cambios causados por la eliminación.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Configure datos de prueba
            cells["A1"].Formula = "=A5";
            cells["A5"].Value = 10;
            
            // Agregar formato condicional
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            fcc.Add(CellArea.CreateCellArea(0, 3, 1, 4), FormatConditionType.Expression,
                OperatorType.Equal, "=A8>0", "");

            // Cree y asigne el monitor
            CustomFormulaChangeMonitor monitor = new CustomFormulaChangeMonitor();
            DeleteOptions options = new DeleteOptions
            {
                FormulaChangeMonitor = monitor,
                UpdateReference = true
            };

            // Elimine la fila que debería desencadenar cambios en las fórmulas
            cells.DeleteRows(2, 1, options);

            // Salida de resultados de monitoreo
            Console.WriteLine("Cell formula changes detected: " + monitor.CellChangesDetected);
            Console.WriteLine("Format condition changes detected: " + monitor.FormatConditionChangesDetected);
        }
    }

    public class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
    {
        public bool CellChangesDetected { get; private set; }
        public bool FormatConditionChangesDetected { get; private set; }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            CellChangesDetected = true;
            Console.WriteLine($"Cell formula changed at Sheet {sheetIndex}, Row {rowIndex}, Column {columnIndex}");
        }

        public override void OnFormatConditionFormulaChanged(FormatCondition fc)
        {
            FormatConditionChangesDetected = true;
            Console.WriteLine("Format condition formula changed");
        }
    }
}
```

### Ver también

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [DeleteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


