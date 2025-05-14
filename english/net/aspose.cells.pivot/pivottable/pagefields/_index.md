---
title: PivotTable.PageFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as page fields
type: docs
url: /net/aspose.cells.pivot/pivottable/pagefields/
---
## PivotTable.PageFields property

Returns a PivotFields object that are currently shown as page fields.

```csharp
public PivotFieldCollection PageFields { get; }
```

### Examples

```csharp
// Called: Aspose.Cells.Pivot.PivotFieldCollection pivotFieldCollection = _PivotTable.PageFields;
public static string PivotTable_Property_PageFields(ref PivotTable _PivotTable)
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

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


