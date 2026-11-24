---
title: "ReferredArea.GetValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReferredArea-Methode. Ruft den Zellenwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs ab."
type: docs
url: /de/net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

Ermittelt den Zellenwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | Int32 | Zeilenversatz von der Startzeile dieses Bereichs. |
| colOffset | Int32 | Spaltenversatz von der Startzeile dieses Bereichs |

### Rückgabewert

"#REF!" wenn dieser Bereich ungültig ist; "#N/A" wenn der angegebene Versatz außerhalb dieses Bereichs liegt; andernfalls den Zellenwert an der angegebenen Position zurückgeben.

### Beispiele

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

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

Ermittelt den Zellenwert mit dem angegebenen Versatz von der oberen linken Ecke dieses Bereichs.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowOffset | Int32 | Zeilenversatz von der Startzeile dieses Bereichs. |
| colOffset | Int32 | Spaltenversatz von der Startzeile dieses Bereichs |
| calculateFormulas | Boolean | Ob es rekursiv berechnet wird, wenn die angegebene Referenz eine Formel ist |

### Rückgabewert

"#REF!" wenn dieser Bereich ungültig ist; "#N/A" wenn der angegebene Versatz außerhalb dieses Bereichs liegt; andernfalls den Zellenwert an der angegebenen Position zurückgeben.

### Beispiele

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

### Siehe auch

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


