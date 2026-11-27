---
title: "PivotField.GroupSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Hämtar grupperingens inställningar för pivottfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/groupsettings/
---
## PivotField.GroupSettings property

Hämtar gruppinställningarna för pivotfältet.

```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```

### Anmärkningar

Om detta fält inte är grupperat returneras Null.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyGroupSettingsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Åtkomst till det andra basfältet (förutsatt att det finns)
            if (pivotTable.BaseFields.Count > 1)
            {
                PivotField pivotField = pivotTable.BaseFields[1];
                
                // Kontrollera om fältet har grupperingens inställningar
                if (pivotField.GroupSettings != null)
                {
                    Console.WriteLine("Field has grouping enabled");
                    Console.WriteLine("Group type: " + pivotField.GroupSettings.Type);
                }
                else
                {
                    Console.WriteLine("Field has no grouping settings");
                }
                
                // Exempel på gruppering av ett numeriskt fält
                if (pivotField.GroupSettings == null && 
                    pivotField.PivotItems.Count > 0 && 
                    pivotField.PivotItems[0].Value is double)
                {
                    // Gruppera efter numeriskt intervall (10-enhetsintervall)
                    pivotField.GroupBy(10.0, false);
                    Console.WriteLine("Field grouped by numeric range");
                }
            }
            
            // Spara den modifierade arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


