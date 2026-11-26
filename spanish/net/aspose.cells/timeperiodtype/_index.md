---
title: "Enum TimePeriodType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.TimePeriodType. Utilizado en una regla de formato condicional FormatConditionType.TimePeriod. Estos son períodos de tiempo dinámicos que cambian según la fecha en que se actualiza / aplica el formato condicional."
type: docs
url: /es/net/aspose.cells/timeperiodtype/
---
## TimePeriodType enumeration

Se utiliza en una regla de formato condicional FormatConditionType.TimePeriod. Estos son períodos de tiempo dinámicos, que cambian según la fecha en que se actualiza / aplica el formato condicional.

```csharp
public enum TimePeriodType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Today | `0` | Fecha de hoy. |
| Yesterday | `1` | Fecha de ayer. |
| Tomorrow | `2` | Fecha de mañana. |
| Last7Days | `3` | Una fecha en los últimos siete días. |
| ThisMonth | `4` | Una fecha que ocurre en este mes calendario. |
| LastMonth | `5` | Una fecha que ocurre en el último mes del calendario. |
| NextMonth | `6` | Una fecha que ocurre en el próximo mes del calendario. |
| ThisWeek | `7` | Una fecha que ocurre esta semana. |
| LastWeek | `8` | Una fecha que ocurre la semana pasada. |
| NextWeek | `9` | Una fecha que ocurre la próxima semana. |
| ThisYear | `10` | Una fecha que ocurre este año. Solo para .ods. |
| LastYear | `11` | Una fecha que ocurre el año pasado. Solo para .ods. |
| NextYear | `12` | Una fecha que ocurre el próximo año. Solo para .ods. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TimePeriodTypeDemo
    {
        public static void TimePeriodTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una regla de formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Definir el área de celdas para el formato condicional
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Agregar una condición para el período de tiempo
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // Establecer el tipo de período de tiempo
            fc.TimePeriod = TimePeriodType.Today;

            // Guarda el libro de trabajo
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


