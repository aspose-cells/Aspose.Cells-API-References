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
// Called: validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
private void Method_CellArea_(int mode)
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = (Aspose.Cells.ValidationType.List);
            validation.InCellDropDown = (true);
            validation.Formula1 = (&quot;=TestRange&quot;);
            validation.AlertStyle = (ValidationAlertType.Warning);
            validation.ErrorTitle = (&quot;Error&quot;);
            validation.ErrorMessage = (&quot;Set a valid value&quot;);
            Cells cells = sheet.Cells;
            Cell cell = cells[0, 0];
            cell.Value = (&quot;CellValue0&quot;);
            for (int i = 1; i &lt; 1022; i++)
            {
                cell = cells[i, 0];
                cell.Value = (&quot;CellValue&quot; + i);
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
                info = &quot;NormalAdd&quot;;
            }
            else if(mode == 1)
            {
                info = &quot;NoMerge&quot;;
            }
            else
            {
                info = &quot;MergeOnSave&quot;;
                saveOptions.MergeAreas = true;
            }

            //wb = Util.ReSave(wb, saveOptions, new LoadOptions());
            wb.Save(Constants.destPath + &quot;J41427_&quot; + info + &quot;.xls&quot;, saveOptions);
            wb = new Workbook(Constants.destPath + &quot;J41427_&quot; + info + &quot;.xls&quot;);
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
            validation.Formula1 = (&quot;=TestRange&quot;);
            validation.AlertStyle = (ValidationAlertType.Warning);
            validation.ErrorTitle = (&quot;Error&quot;);
            validation.ErrorMessage = (&quot;Set a valid value&quot;);
            Cells cells = sheet.Cells;
            Cell cell = cells[0, 0];
            cell.Value = (&quot;CellValue0&quot;);
            for (int i = 1; i &lt; 1022; i++)
            {
                cell = cells[i, 0];
                cell.Value = (&quot;CellValue&quot; + i);
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
                info = &quot;NormalAdd&quot;;
            }
            else if(mode == 1)
            {
                info = &quot;NoMerge&quot;;
            }
            else
            {
                info = &quot;MergeOnSave&quot;;
                saveOptions.MergeAreas = true;
            }

            //wb = Util.ReSave(wb, saveOptions, new LoadOptions());
            wb.Save(Constants.destPath + &quot;J41427_&quot; + info + &quot;.xls&quot;, saveOptions);
            wb = new Workbook(Constants.destPath + &quot;J41427_&quot; + info + &quot;.xls&quot;);
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


