---
title: "FormatConditionCollection.AddCondition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatConditionCollection. Agrega una condición de formato"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

Agrega una condición de formato.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | FormatConditionType | El tipo de condición de formato. |
| operatorType | OperatorType | El tipo de operador |
| formula1 | String | El valor o expresión asociado con el formato condicional. Si el valor de entrada comienza con '=', se tomará como una fórmula. De lo contrario se tomará como un valor simple (texto, número, bool). Para valores de texto que comienzan con '=', el usuario puede ingresarlo como fórmula en el formato: "=\"=...\"". |
| formula2 | String | El valor o expresión asociado con el formato condicional. El formato de entrada es el mismo que formula1 |

### Valor de retorno

Índice del objeto de condición de formato;

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeOperatorTypDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;
            fcs.AddArea(ca);
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Red;
            
            conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "0", "50");
            fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Green;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

Agregar una condición de formato.

```csharp
public int AddCondition(FormatConditionType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | FormatConditionType | Tipo de condición de formato. |

### Valor de retorno

Índice del objeto de condición de formato;

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear condiciones de formato
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            
            // Agregar rango
            CellArea area = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 5,
                EndColumn = 5
            };
            conditions.AddArea(area);

            // Agregar condiciones (devuelve índice int)
            conditions.AddCondition(FormatConditionType.ColorScale);
            conditions.AddCondition(FormatConditionType.IconSet);
            conditions.AddCondition(FormatConditionType.DataBar);

            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


