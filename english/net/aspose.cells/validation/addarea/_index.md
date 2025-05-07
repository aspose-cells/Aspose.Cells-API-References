---
title: Validation.AddArea
second_title: Aspose.Cells for .NET API Reference
description: Validation method. Applies the validation to the area
type: docs
url: /net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

Applies the validation to the area.

```csharp
public void AddArea(CellArea cellArea)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area. |

### Remarks

It is equivalent to use `AddArea` with checking intersection and edge.

### Examples

```csharp
// Called: vldt.AddArea(item);
[Test]
        public void Method_CellArea_()
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

---

## AddArea(CellArea, bool, bool) {#addarea_1}

Applies the validation to the area.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area. |
| checkIntersection | Boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that the added area does not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | Boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if given area will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that the added area is not the top-left one, this parameter can be set as false for performance consideration. |

### Remarks

In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.

### Examples

```csharp
// Called: validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0), false, false);
private void Method_Boolean_(int mode)
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = (Aspose.Cells.ValidationType.List);
            validation.InCellDropDown = (true);
            validation.Formula1 = ("=TestRange");
            validation.AlertStyle = (ValidationAlertType.Warning);
            validation.ErrorTitle = ("Error");
            validation.ErrorMessage = ("Set a valid value");
            Cells cells = sheet.Cells;
            Cell cell = cells[0, 0];
            cell.Value = ("CellValue0");
            for (int i = 1; i < 1022; i++)
            {
                cell = cells[i, 0];
                cell.Value = ("CellValue" + i);
                if(mode == 0)
                {
                    validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
                }
                else
                {
                    validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0), false, false);
                }
            }
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            string info;
            if (mode == 0)
            {
                info = "NormalAdd";
            }
            else if(mode == 1)
            {
                info = "NoMerge";
            }
            else
            {
                info = "MergeOnSave";
                saveOptions.MergeAreas = true;
            }

            //wb = Util.ReSave(wb, saveOptions, new LoadOptions());
            wb.Save(Constants.destPath + "J41427_" + info + ".xls", saveOptions);
            wb = new Workbook(Constants.destPath + "J41427_" + info + ".xls");
            vc = wb.Worksheets[0].Validations;
            if(mode == 1)
            {
                Assert.AreEqual(2, vc.Count, info);
                CellArea[] cas = vc[0].Areas;
                Assert.AreEqual(1, cas.Length, info);
                AssertHelper.checkCellArea(0, 0, 1020, 0, cas[0], info);
                cas = vc[1].Areas;
                Assert.AreEqual(1, cas.Length, info);
                AssertHelper.checkCellArea(1021, 0, 1021, 0, cas[0], info);
            }
            else
            {
                Assert.AreEqual(1, vc.Count, info);
                CellArea[] cas = vc[0].Areas;
                Assert.AreEqual(1, cas.Length, info);
                AssertHelper.checkCellArea(0, 0, 1021, 0, cas[0], info);
            }
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


