---
title: Cell.DateTimeValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the DateTime value contained in the cell
type: docs
url: /net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Gets the DateTime value contained in the cell.

```csharp
public DateTime DateTimeValue { get; }
```

### Examples

```csharp
// Called: newCell.Value = (oldCell.DateTimeValue);
[Test]
        public void Property_DateTimeValue()
        {
            Workbook book = new Workbook(Constants.sourcePath + &quot;CellsJava42740.xlsx&quot;);
            //Workbook book = new Workbook(path + &quot;Book1.xlsx&quot;); 
            Workbook newWb = new Workbook();
            Worksheet oldWs = book.Worksheets[0];
            Worksheet newWs = newWb.Worksheets[0];

            ValidationCollection oldValidationCollection = oldWs.Validations;
            ValidationCollection newValidationCollection = newWs.Validations;
            int vCount = oldValidationCollection.Count;

            for (int i = 0; i &lt; vCount; i++)
            {
                Validation oldValidation = oldValidationCollection[i];
                // newValidationCollection.Add(oldValidation);
                CellArea[] areas = oldValidation.Areas;
                int index = newValidationCollection.Add(areas[0]);
                Validation newValidation = newValidationCollection[i];
                newValidation.Copy(oldValidation, null);
            }

            Cells oldCells = oldWs.Cells;
            Cells newCells = newWs.Cells;
            int maxRow = oldCells.MaxDataRow;
            int maxCol = oldCells.MaxDataColumn;

            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = (true);

            for (int r = 0; r &lt;= maxRow; r++)
            {
                for (int c = 0; c &lt;= maxCol; c++)
                {
                    try
                    {
                        Cell oldCell = oldCells[r, c];
                        Cell newCell = newCells[r, c];

                        CellValueType type = oldCell.Type;

                        switch (type)
                        {
                            case CellValueType.IsNumeric:
                                newCell.Value = (oldCell.DoubleValue);
                                break;
                            case CellValueType.IsDateTime:
                                newCell.Value = (oldCell.DateTimeValue);
                                break;
                            case CellValueType.IsString:
                                newCell.Value = (oldCell.StringValue);
                                break;
                        }

                        newCell.SetStyle(oldCell.GetDisplayStyle());
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine(ex);
                    }
                }
            }

            Util.ReSave(newWb, SaveFormat.Xlsx);
            //newWb.Save(Constants.destPath + &quot;CellsJava42740.xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


