---
title: "Worksheet.FreezePanes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet‑metod. Fryser rutor på den angivna cellen i arbetsbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/freezepanes/
---
## FreezePanes(int, int, int, int) {#freezepanes}

Fryser rutor vid den angivna cellen i kalkylbladet.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex. |
| column | Int32 | Kolumnindex. |
| freezedRows | Int32 | Antal synliga rader i översta rutan, högst radindex. |
| freezedColumns | Int32 | Antal synliga kolumner i vänstra rutan, högst kolumnindex. |

### Anmärkningar

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

De två första parametrarna anger den frysta positionen och de två sista parametrarna anger området som är fryst i den vänstra övre rutan.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Frys rutor på rad 3, kolumn 3, med 3 frysta rader och 3 frysta kolumner
            worksheet.FreezePanes(3, 3, 3, 3);
            
            // Spara arbetsboken
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## FreezePanes(string, int, int) {#freezepanes_1}

Fryser rutor vid den angivna cellen i kalkylbladet.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |
| freezedRows | Int32 | Antal synliga rader i översta rutan, högst radindex. |
| freezedColumns | Int32 | Antal synliga kolumner i vänstra rutan, högst kolumnindex. |

### Anmärkningar

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Frys rutor på "C3" med 3 frysta rader och 3 frysta kolumner
            worksheet.FreezePanes("C3", 3, 3);

            // Spara arbetsboken
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


