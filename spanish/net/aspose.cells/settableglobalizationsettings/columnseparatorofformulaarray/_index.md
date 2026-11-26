---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SettableGlobalizationSettings. Obtiene el separador para los elementos en los datos de fila de matrices en la fórmula"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

Obtiene el separador para los elementos en los datos de fila de la matriz en la fórmula.

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una instancia de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Mostrar el valor actual de ColumnSeparatorOfFormulaArray
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // Establecer un nuevo valor para ColumnSeparatorOfFormulaArray
            settings.SetColumnSeparatorOfFormulaArray(';');

            // Aplicar la configuración al libro de trabajo
            workbook.Settings.GlobalizationSettings = settings;

            // Crear una fórmula de matriz con el separador personalizado usando SetArrayFormula
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // Calcular fórmulas
            workbook.CalculateFormula();

            // Mostrar el resultado
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // Guarda el libro de trabajo
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


