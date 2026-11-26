---
title: "GlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlobalizationSettings. Obtiene el separador para los elementos en los datos de filas de matrices en la fórmula"
type: docs
url: /es/net/aspose.cells/globalizationsettings/columnseparatorofformulaarray/
---
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property

Obtiene el separador para los elementos en los datos de fila de la matriz en la fórmula.

```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear configuraciones de globalización personalizadas con separador de columna sobrescrito
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Mostrar el valor actual del separador de columna
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
                globalizationSettings.ColumnSeparatorOfFormulaArray);

            // Crear fórmula de matriz usando separador personalizado
            Cell cell = worksheet.Cells["A1"];
            cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator

            // Verificar el almacenamiento de la fórmula (mostraría puntos y comas en la cadena de fórmula real)
            Console.WriteLine("Stored array formula: " + cell.Formula);

            // Guardar el libro de trabajo modificado
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ColumnSeparatorOfFormulaArray => ';';
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


