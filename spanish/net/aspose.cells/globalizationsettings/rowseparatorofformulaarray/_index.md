---
title: "GlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlobalizationSettings. Obtiene el separador para filas en datos de matriz en la fórmula"
type: docs
url: /es/net/aspose.cells/globalizationsettings/rowseparatorofformulaarray/
---
## GlobalizationSettings.RowSeparatorOfFormulaArray property

Obtiene el separador para las filas en los datos de matriz en la fórmula.

```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con configuraciones de globalización personalizadas
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceda a la instancia de configuración de globalización personalizada
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            // Muestre el valor actual de RowSeparatorOfFormulaArray
            Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Cree una fórmula de matriz usando el separador de filas personalizado
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator

            // Calcule la fórmula para demostrar el análisis correcto
            workbook.CalculateFormula();

            // Mostrar resultados
            Console.WriteLine("Array formula using custom separator: " + cell.Formula);
            Console.WriteLine("Calculated result: " + cell.Value);

            // Guarda el libro de trabajo
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }

    // Implementación personalizada de GlobalizationSettings que sobrescribe el separador de filas
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override char RowSeparatorOfFormulaArray => '|';
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


