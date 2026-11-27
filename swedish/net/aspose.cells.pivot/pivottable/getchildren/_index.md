---
title: "PivotTable.GetChildren"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable metod. Hämtar de underordnade pivottabellerna som använder denna PivotTable-data som datakälla"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/getchildren/
---
## PivotTable.GetChildren method

Hämtar de underordnade pivottabellerna som använder denna PivotTable-data som datakälla.

```csharp
[Obsolete("Use PivotTable.GetDependentPivotTables() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotTable[] GetChildren()
```

### Returvärde

PivotTable-arrayobjektet

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotTable.GetDependentPivotTables() metod. Denna metod kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetChildrenDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(300);

            // Skapa huvudpivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "MainPivotTable");
            PivotTable mainPivotTable = pivotTables[index];
            mainPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            mainPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Skapa underordnad pivottabell
            index = pivotTables.Add("A1:B4", "E10", "ChildPivotTable");
            PivotTable childPivotTable = pivotTables[index];
            childPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            childPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Etablera relation genom att dela grundfält
            foreach (PivotField field in mainPivotTable.BaseFields)
            {
                childPivotTable.BaseFields.Add(field);
            }

            // Demonstrera GetChildren() metod
            Console.WriteLine("Child Pivot Tables:");
            foreach (PivotTable child in mainPivotTable.GetChildren())
            {
                Console.WriteLine("Child Pivot Table Name: " + child.Name);
                Console.WriteLine("Child Pivot Table Location: " + child.TableRange1);
            }
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


