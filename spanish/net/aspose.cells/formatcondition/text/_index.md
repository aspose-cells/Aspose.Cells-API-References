---
title: "FormatCondition.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. El valor de texto en una regla de formato condicional que contiene texto. Válido solo para el tipo containsText, notContainsText, beginsWith y endsWith. El valor predeterminado es null"
type: docs
url: /es/net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

El valor de texto en una regla de formato condicional "text contains". Válido solo para type = containsText, notContainsText, beginsWith y endsWith. El valor predeterminado es null.

```csharp
public string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTextDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar formato condicional
            ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
            int collectionIndex = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];

            // Agregar condición de texto
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            
            // Establece la propiedad de texto (demostrando texto en ruso)
            formatCondition.Text = "вс";

            // Aplicar estilo de formato
            Style style = formatCondition.Style;
            style.BackgroundColor = Color.Red;
            formatCondition.Style = style;

            // Aplicar a la celda A1
            formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));

            // Guardar y verificar
            string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("FormatCondition Text property demo completed successfully.");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


