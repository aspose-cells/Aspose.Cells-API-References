---
title: "ConditionalFormattingIcon.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingIcon. Obtiene y establece el tipo del conjunto de íconos"
type: docs
url: /es/net/aspose.cells/conditionalformattingicon/type/
---
## ConditionalFormattingIcon.Type property

Obtiene y establece el tipo de conjunto de íconos.

```csharp
public IconSetType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingIconPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Agregar formato condicional con conjunto de iconos
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fc = cfs[index];
            fc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 2, EndColumn = 0 });
            
            int conditionIndex = fc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fc[conditionIndex];
            condition.IconSet.Type = IconSetType.Symbols3;
            
            // Aplicar formato y calcular
            workbook.CalculateFormula();

            // Obtener el resultado del formato y demostrar la propiedad Type
            Cell cell = worksheet.Cells["A2"];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            
            Console.WriteLine("Icon Set Type: " + formattingResult.ConditionalFormattingIcon.Type);
            Console.WriteLine("Icon Index: " + formattingResult.ConditionalFormattingIcon.Index);
        }
    }
}
```

### Ver también

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


