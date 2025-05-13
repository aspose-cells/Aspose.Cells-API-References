---
title: Validation.RemoveArea
second_title: Aspose.Cells for .NET API Reference
description: Validation method. Remove the validation settings in the range
type: docs
url: /net/aspose.cells/validation/removearea/
---
## Validation.RemoveArea method

Remove the validation settings in the range.

```csharp
public void RemoveArea(CellArea cellArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | the areas where this validation settings should be removed. |

### Examples

```csharp
// Called: vldt.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
public void Validation_Method_RemoveArea()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    Validation vldt = sheet.Validations[sheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
    vldt.Operator = OperatorType.GreaterThan;
    vldt.Formula1 = "F3";

    vldt.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
    Assert.AreEqual(2, vldt.Areas.Length, "Area count after changing base");
    Assert.AreEqual("=F3", vldt.Formula1, "Formula1 after changing base, now total 2 areas");
    vldt.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
    Assert.AreEqual(1, vldt.Areas.Length, "Area count after removing base");
    Assert.AreEqual("=F3", vldt.Formula1, "Formula1 after removing base");

    CellArea[] areas = new CellArea[8000];
    for (int i = 0; i < areas.Length; i++)
    {
        areas[i] = CellArea.CreateCellArea(6 + (i<<1), 3, 6 + (i<<1), 4);
    }
    TimePerformance monitor = new TimePerformance(5);
    monitor.StartPerfTest();
    foreach (CellArea item in areas)
    {
        vldt.AddArea(item);
    }
    Console.WriteLine("PerfBase of adding one by one: " + monitor.GenPerfBase());
    //monitor.FinishPerfTest("Validation.AddArea");
    Assert.AreEqual("=F3", vldt.Formula1, "Formula1 after adding one by one without changing base");
    vldt.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
    Assert.AreEqual(areas.Length + 2, vldt.Areas.Length, "Area count before removing base");
    Assert.AreEqual("=F3", vldt.Formula1,
        "Formula1 after changing base, now total 802 areas");
    vldt.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
    Assert.AreEqual(areas.Length + 1, vldt.Areas.Length, "Area count after removing base");
    Assert.AreEqual("=F3", vldt.Formula1,
        "Formula1 after removing base, now total 801 areas");

    monitor.StartPerfTest();
    foreach (CellArea item in areas)
    {
        vldt.RemoveArea(item);
    }
    Console.WriteLine("PerfBase of removing one by one: " + monitor.GenPerfBase());
    Assert.AreEqual(1, vldt.Areas.Length, "Area count after removing one by one");
    Assert.AreEqual("=F3", vldt.Formula1, "Formula1 after removing one by one without changing base");

    monitor.StartPerfTest();
    areas[areas.Length/2] = CellArea.CreateCellArea(3, 3, 3, 4);
    vldt.AddAreas(areas, true, true);
    Console.WriteLine("PerfBase of bulk adding: " + monitor.GenPerfBase());
    Assert.AreEqual(areas.Length + 1, vldt.Areas.Length, "Area count after bulk adding");
    Assert.AreEqual("=F3", vldt.Formula1,
        "Formula1 after changing base by bulk adding, now total 801 areas");

    monitor.StartPerfTest();
    vldt.RemoveAreas(areas);
    Console.WriteLine("PerfBase of bulk removing: " + monitor.GenPerfBase());
    Assert.AreEqual(1, vldt.Areas.Length, "Area count after bulk removing");
    Assert.AreEqual("=F3", vldt.Formula1, "Formula1 after changing base, now total 1 area");
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


