---
title: "ConditionalFormattingCollection.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ConditionalFormattingCollection. Copia el formato condicional"
type: docs
url: /es/net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

Copia el formato condicional.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | El formato condicional |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Crear un libro de trabajo fuente con formato condicional
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];

            // Agregar formato condicional de ejemplo a la hoja fuente
            int index = sourceSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Crear y aplicar estilo a la condición de formato
            Style style = sourceWorkbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Red;
            FormatCondition fc = fcc[0];
            fc.Style = style;

            // Aplicar a un rango
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 5;
            area.StartColumn = 0;
            area.EndColumn = 5;
            fcc.AddArea(area);

            // Copiar formato condicional de la fuente al destino
            destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);

            // Guarda el libro de trabajo
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


