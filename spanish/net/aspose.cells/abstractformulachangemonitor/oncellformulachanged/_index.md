---
title: "AbstractFormulaChangeMonitor.OnCellFormulaChanged"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractFormulaChangeMonitor. El evento que se disparará cuando la fórmula en una celda cambie"
type: docs
url: /es/net/aspose.cells/abstractformulachangemonitor/oncellformulachanged/
---
## AbstractFormulaChangeMonitor.OnCellFormulaChanged method

El evento que se activará cuando la fórmula en una celda cambie.

```csharp
public virtual void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | El índice de hoja de la celda modificada |
| rowIndex | Int32 | El índice de fila de la celda modificada |
| columnIndex | Int32 | El índice de columna de la celda modificada |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo : AbstractFormulaChangeMonitor
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de nuestra clase de demostración que hereda de AbstractFormulaChangeMonitor
            var monitor = new AbstractFormulaChangeMonitorMethodOnCellFormulaChangedWithInt32Int32Int32Demo();

            // Establecer alguna fórmula en una celda para desencadenar el cambio
            worksheet.Cells["A1"].Formula = "=SUM(B1:B10)";

            try
            {
                // Llamar a OnCellFormulaChanged con índice de hoja 0, fila 0, columna 0 (A1)
                monitor.OnCellFormulaChanged(0, 0, 0);

                Console.WriteLine("OnCellFormulaChanged called successfully for cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OnCellFormulaChanged method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("OnCellFormulaChangedDemo.xlsx");
        }

        public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
        {
            // Implementación para manejar el cambio de fórmula
            Console.WriteLine($"Formula changed in sheet {sheetIndex} at row {rowIndex}, column {columnIndex}");
        }

    }
}
```

### Ver también

* class [AbstractFormulaChangeMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


