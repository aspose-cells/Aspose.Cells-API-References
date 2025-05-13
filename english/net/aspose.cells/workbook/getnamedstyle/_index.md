---
title: Workbook.GetNamedStyle
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Gets the named style in the style pool
type: docs
url: /net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Gets the named style in the style pool.

```csharp
public Style GetNamedStyle(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | name of the style |

### Return Value

named style, maybe null.

### Examples

```csharp
// Called: style1 = excel.GetNamedStyle("Number7");
private void Workbook_Method_GetNamedStyle(Aspose.Cells.Cells cells, Workbook excel, DataTable dtInvoice, int startRow)
		{
			Style style1, style2, style3;
			style1 = excel.GetNamedStyle("Number7");
			style2 = excel.GetNamedStyle("Number9");
			style3 = excel.GetNamedStyle("Center");

			for(int i = 0; i < dtInvoice.Rows.Count; i ++)
			{
				cells[startRow + i, 0].PutValue((int)dtInvoice.Rows[i]["ProductID"]);
				cells[startRow + i, 0].SetStyle(style3);
				cells[startRow + i, 1].PutValue((string)dtInvoice.Rows[i]["ProductName"]);
				cells[startRow + i, 3].PutValue((short)dtInvoice.Rows[i]["Quantity"]);
				cells[startRow + i, 4].PutValue((double)(decimal)dtInvoice.Rows[i]["UnitPrice"]);
				cells[startRow + i, 4].SetStyle(style1);
				cells[startRow + i, 5].PutValue((float)dtInvoice.Rows[i]["Discount"]);
				cells[startRow + i, 5].SetStyle(style2);
				cells[startRow + i, 6].PutValue((double)(decimal)dtInvoice.Rows[i]["ExtendedPrice"]);
				cells[startRow + i, 6].SetStyle(style1);
			}
		}
```

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


