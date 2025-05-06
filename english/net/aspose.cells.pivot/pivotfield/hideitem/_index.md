---
title: PivotField.HideItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the specific PivotItem in a data field is hidden
type: docs
url: /net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Sets whether the specific PivotItem in a data field is hidden.

```csharp
public void HideItem(int index, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the pivotItem in the pivotField. |
| isHidden | Boolean | whether the specific PivotItem is hidden |

### Examples

```csharp
// Called: pf.HideItem(i, pf.Items[i] != &amp;quot;PO-23-05&amp;quot;);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + &quot;wec3.xls&quot;);
            Workbook wb1 = new Workbook(Constants.openPivottablePath + &quot;basis+PO.xls&quot;);
            Worksheet wsin = wb.Worksheets[0];
            PivotTable pt = wsin.PivotTables[&quot;Draaitabel2&quot;];
            PivotField pf = pt.RowFields[0];
            for (int i = 0; i &lt; pf.ItemCount; i++)
            {
                pf.HideItem(i, pf.Items[i] != &quot;PO-23-05&quot;);
            }

            pt.CalculateData();
            pt.CalculateRange();

            Worksheet wsout = wb1.Worksheets[&quot;Ambulante begeleiding&quot;];
            Aspose.Cells.Range rin = wsin.Cells.CreateRange(pt.TableRange1.StartRow + 1, pt.TableRange1.StartColumn, pt.TableRange1.EndRow - pt.TableRange1.StartRow - 1, pt.TableRange1.EndColumn - pt.TableRange1.StartColumn + 1);
            Aspose.Cells.Range rout = wsout.Cells.CreateRange(2, 0, pt.TableRange1.EndRow - pt.TableRange1.StartRow - 1, pt.TableRange1.EndColumn - pt.TableRange1.StartColumn + 1);
            rout.CopyData(rin);
            rout.CopyStyle(rin);


            wb.Save(Constants.savePivottablePath + &quot;40113-1.xls&quot;);
            wb1.Save(Constants.savePivottablePath + &quot;40113-2.xls&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

Sets whether the specific PivotItem in a data field is hidden.

```csharp
public void HideItem(string itemValue, bool isHidden)
```

| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | String | the value of the pivotItem in the pivotField. |
| isHidden | Boolean | whether the specific PivotItem is hidden |

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


