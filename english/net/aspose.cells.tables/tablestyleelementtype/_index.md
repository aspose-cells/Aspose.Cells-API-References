---
title: Enum TableStyleElementType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Tables.TableStyleElementType enum. Represents the Table or PivotTable style element type
type: docs
url: /net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

Represents the Table or PivotTable style element type.

```csharp
public enum TableStyleElementType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| BlankRow | `18` | Table style element that applies to PivotTable's blank rows. |
| FirstColumn | `8` | Table style element that applies to table's first column. |
| FirstColumnStripe | `3` | Table style element that applies to table's first column stripes. |
| FirstColumnSubheading | `22` | Table style element that applies to PivotTable's first column subheading. |
| FirstHeaderCell | `11` | Table style element that applies to table's first header row cell. |
| FirstRowStripe | `5` | Table style element that applies to table's first row stripes. |
| FirstRowSubheading | `25` | Table style element that applies to PivotTable's first row subheading. |
| FirstSubtotalColumn | `15` | Table style element that applies to PivotTable's first subtotal column. |
| FirstSubtotalRow | `19` | Table style element that applies to pivot table's first subtotal row. |
| GrandTotalColumn | `28` | Table style element that applies to pivot table's grand total column. |
| GrandTotalRow | `29` | Table style element that applies to pivot table's grand total row. |
| FirstTotalCell | `13` | Table style element that applies to table's first total row cell. |
| HeaderRow | `9` | Table style element that applies to table's header row. |
| LastColumn | `7` | Table style element that applies to table's last column. |
| LastHeaderCell | `12` | Table style element that applies to table's last header row cell. |
| LastTotalCell | `14` | Table style element that applies to table's last total row cell. |
| PageFieldLabels | `1` | Table style element that applies to pivot table's page field labels. |
| PageFieldValues | `2` | Table style element that applies to pivot table's page field values. |
| SecondColumnStripe | `4` | Table style element that applies to table's second column stripes. |
| SecondColumnSubheading | `23` | Table style element that applies to pivot table's second column subheading. |
| SecondRowStripe | `6` | Table style element that applies to table's second row stripes. |
| SecondRowSubheading | `26` | Table style element that applies to pivot table's second row subheading. |
| SecondSubtotalColumn | `16` | Table style element that applies to PivotTable's second subtotal column. |
| SecondSubtotalRow | `20` | Table style element that applies to PivotTable's second subtotal row. |
| ThirdColumnSubheading | `24` | Table style element that applies to PivotTable's third column subheading. |
| ThirdRowSubheading | `27` | Table style element that applies to PivotTable's third row subheading. |
| ThirdSubtotalColumn | `17` | Table style element that applies to pivot table's third subtotal column. |
| ThirdSubtotalRow | `21` | Table style element that applies to PivotTable's third subtotal row. |
| TotalRow | `10` | Table style element that applies to table's total row. |
| WholeTable | `0` | Table style element that applies to table's entire content. |

### Examples

```csharp
// Called: index1 = elements.Add(TableStyleElementType.LastColumn);
public static void Tables_Type_TableStyleElementType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create styles for the first and last columns
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;

            // Define a custom table style name
            string tableStyleName = "Custom1";

            // Access the table styles collection
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            // Add a new table style to the collection
            int index1 = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[index1];

            // Access the table style elements collection
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Add and set style for the first column
            index1 = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[index1];
            element.SetElementStyle(firstColumnStyle);

            // Add and set style for the last column
            index1 = elements.Add(TableStyleElementType.LastColumn);
            element = elements[index1];
            element.SetElementStyle(lastColumnStyle);

            // Access the cells of the first worksheet
            Cells cells = workbook.Worksheets[0].Cells;

            // Populate the first row with column names
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }

            // Populate the rest of the cells with sample data
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Add a table to the worksheet
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Apply the custom table style to the table
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            // Save the workbook
            workbook.Save("TableStyleExample.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


