---
title: PivotItem.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets and Sets whether the pivot item is hidden
type: docs
url: /net/aspose.cells.pivot/pivotitem/ishidden/
---
## PivotItem.IsHidden property

Gets and Sets whether the pivot item is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: _Ret += "Name: " + _PivotItem.Name + " - Hidden: " + _PivotItem.IsHidden.ToString() + Environment.NewLine;
public static string Property_IsHidden(ref PivotTable _PivotTable)
        {
            //PivotItemCollection items;
            PivotItem _PivotItem;
            string _strItemActualPivotField;
            string _Ret = "";
            Aspose.Cells.Pivot.PivotField _PivotField = null;
            Aspose.Cells.Pivot.PivotFieldCollection pivotFieldCollection = _PivotTable.PageFields;

            //Select the Item
            for (int y = 0; y < pivotFieldCollection.Count; y++)
            {
                _PivotField = pivotFieldCollection[y];
                //items = _PivotField.PivotItems;

                _Ret += "-----------------------------------" + _PivotField.Name + Environment.NewLine;

                for (int i = 0; i < _PivotField.PivotItems.Count; i++)
                {
                    _PivotItem = _PivotField.PivotItems[i];
                    _strItemActualPivotField = (_PivotItem.Value == null ? "" : _PivotItem.Value.ToString());

                    _Ret += "Name: " + _PivotItem.Name + " - Hidden: " + _PivotItem.IsHidden.ToString() + Environment.NewLine;
                }

                //_PivotTable.RefreshData();
                //_PivotTable.CalculateData();
            }
            return _Ret;
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


