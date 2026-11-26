---
title: "FormatConditionCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatConditionCollection. Agrega una condición de formato y el rango de celdas afectado a los FormatConditions. Los FormatConditions pueden contener hasta tres formatos condicionales. No se permiten referencias a otras hojas en las fórmulas del formato condicional"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Agrega una condición de formato y el rango de celdas afectado a los FormatConditions. Los FormatConditions pueden contener hasta tres formatos condicionales. No se permiten referencias a otras hojas en las fórmulas del formato condicional.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | CellArea | Rango de celdas con formato condicional. |
| type | FormatConditionType | Tipo de formato condicional.Puede ser uno de los miembros de FormatConditionType. |
| operatorType | OperatorType | Operador de comparación.Puede ser uno de los miembros de OperatorType. |
| formula1 | String | El valor o expresión asociado con el formato condicional. |
| formula2 | String | El valor o expresión asociado con el formato condicional |

### Valor de retorno

[0]:Formatting condition object index;[1] Effected cell rang index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddWithCellAreaFormatConditionTypeOpeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Rellene datos de ejemplo
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Agregar formato condicional
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            
            // Demostrar el método Add con parámetros especificados
            fcc.Add(
                CellArea.CreateCellArea(0, 0, 4, 0),
                FormatConditionType.Expression,
                OperatorType.None,
                "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
                null
            );

            // Aplicar formato
            int fontSize = wb.DefaultStyle.Font.Size;
            fcc[0].Style.Font.Size = fontSize + 2;

            // Guardar el libro de trabajo para demostrar el resultado
            wb.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


