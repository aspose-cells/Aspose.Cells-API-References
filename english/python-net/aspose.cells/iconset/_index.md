---
title: IconSet class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 900
url: /python-net/aspose.cells/iconset/
is_root: false
---

## IconSet class

Describe the IconSet conditional formatting rule. 
This conditional formatting rule applies icons to cells
according to their values.



The IconSet type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [cf_icons](/cells/python-net/aspose.cells/iconset/cf_icons) | Get the[ConditionalFormattingIcon](/cells/python-net/aspose.cells/conditionalformattingicon) from the collection |
| [cfvos](/cells/python-net/aspose.cells/iconset/cfvos) | Get the CFValueObjects instance. |
| [type](/cells/python-net/aspose.cells/iconset/type) | Get or Set the icon set type to display.<br/>Setting the type will auto check if the current Cfvos's count is<br/>accord with the new type. If not accord, old Cfvos will be cleaned and <br/>default Cfvos will be added. |
| [is_custom](/cells/python-net/aspose.cells/iconset/is_custom) | Indicates whether the icon set is custom.<br/>Default value is false. |
| [show_value](/cells/python-net/aspose.cells/iconset/show_value) | Get or set the flag indicating whether to show the values of the cells on which this icon set is applied.<br/>Default value is true. |
| [reverse](/cells/python-net/aspose.cells/iconset/reverse) | Get or set the flag indicating whether to reverses the default order of the icons in this icon set.<br/>Default value is false. |


### Example 


```
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]

# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]

# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)

# Adds condition.
idx = fcs.add_condition(FormatConditionType.ICON_SET)
fcs.add_area(ca)
cond = fcs[idx]

# Get Icon Set
iconSet = cond.icon_set

# Set Icon Type
iconSet.type = IconSetType.ARROWS3

# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)

# Saving the Excel file
workbook.save("book1.xlsx")

```
### See Also

* module [aspose.cells](../)
