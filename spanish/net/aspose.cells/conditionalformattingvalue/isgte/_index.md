---
title: "ConditionalFormattingValue.IsGTE"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingValue. Obtenga o establezca el indicador Greater Than Or Equal. Úselo solo para conjuntos de íconos; determina si este valor umbral utiliza el operador mayor o igual que. false indica que se usa mayor que en lugar de mayor o igual que. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

Obtenga o establezca la bandera Greater Than Or Equal. Úsela solo para conjuntos de iconos, determina si este valor de umbral utiliza el operador mayor o igual que. 'false' indica que se usa 'greater than' en lugar de 'greater than or equal to'. El valor predeterminado es true.

```csharp
public bool IsGTE { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyIsGTEDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            // Agregar formato condicional
            int index = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[index];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            // Cree un formato de escala de colores
            index = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[index];
            
            // Configure una escala de 2 colores
            fc.ColorScale.Is3ColorScale = false;
            
            // Establezca el formato de valor máximo (demostrando IsGTE)
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            // Establezca el formato de valor mínimo
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


