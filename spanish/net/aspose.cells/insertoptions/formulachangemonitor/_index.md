---
title: "InsertOptions.FormulaChangeMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad InsertOptions. Obtiene/establece el monitor para rastrear los cambios causados por la inserción"
type: docs
url: /es/net/aspose.cells/insertoptions/formulachangemonitor/
---
## InsertOptions.FormulaChangeMonitor property

Obtiene/establece el monitor para rastrear los cambios causados por la inserción.

```csharp
public AbstractFormulaChangeMonitor FormulaChangeMonitor { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsPropertyFormulaChangeMonitorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo con fórmulas
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Formula = "=A1*2";
            worksheet.Cells["B1"].Formula = "=SUM(A1:A2)";

            try
            {
                // Crear instancia de InsertOptions
                InsertOptions options = new InsertOptions();

                // Crear una implementación personalizada de FormulaChangeMonitor
                var monitor = new CustomFormulaChangeMonitor();
                options.FormulaChangeMonitor = monitor;

                // Mostrar el FormulaChangeMonitor actual
                Console.WriteLine("FormulaChangeMonitor is set: " +
                    (options.FormulaChangeMonitor != null));

                // Insertar filas que pueden desencadenar cambios de fórmula
                worksheet.Cells.InsertRows(1, 1, options);

                // Guardar el resultado
                workbook.Save("FormulaChangeMonitorDemo.xlsx");
                Console.WriteLine("FormulaChangeMonitor demonstration completed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Implementación personalizada de AbstractFormulaChangeMonitor
        private class CustomFormulaChangeMonitor : AbstractFormulaChangeMonitor
        {
            public override void OnCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
            {
                Console.WriteLine($"Formula changed at Sheet {sheetIndex}, Cell {rowIndex},{columnIndex}");
            }

            public override void OnFormatConditionFormulaChanged(FormatCondition fc)
            {
                Console.WriteLine($"Format condition formula changed: {fc.Formula1}");
            }
        }
    }
}
```

### Ver también

* class [AbstractFormulaChangeMonitor](../../abstractformulachangemonitor/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


