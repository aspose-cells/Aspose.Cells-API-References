---
title: "ReferredArea.GetValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-metoden. Hämtar cellvärdet med given förskjutning från detta områdes övre vänstra hörn"
type: docs
url: /sv/net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

Hämtar cellvärdet med given offset från det övre vänstra hörnet av detta område.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | radförskjutning från startraden i detta område |
| colOffset | Int32 | kolumnförskjutning från startraden i detta område |

### Returvärde

"#REF!" om detta område är ogiltigt; "#N/A" om angiven förskjutning ligger utanför detta område; annars returneras cellvärdet på given position.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue(5);
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = "=A1";
            
            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreas = cell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                object value = referredAreas[0].GetValue(0, 0);
                Console.WriteLine("Value at (0,0): " + value);
            }
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

Hämtar cellvärdet med given offset från det övre vänstra hörnet av detta område.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | Int32 | radförskjutning från startraden i detta område |
| colOffset | Int32 | kolumnförskjutning från startraden i detta område |
| calculateFormulas | Boolean | Om den ska beräknas rekursivt om den angivna referensen är en formel |

### Returvärde

"#REF!" om detta område är ogiltigt; "#N/A" om angiven förskjutning ligger utanför detta område; annars returneras cellvärdet på given position.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(100);
            sheet.Cells["B1"].PutValue(200);

            workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names["TestRange"];
            name.RefersTo = "=Sheet1!$A$1:$B$1";

            ReferredArea ra = name.GetReferredAreas(true)[0];
            object result = ra.GetValue(0, 0, true);

            Console.WriteLine("Obtained value: " + result);
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


