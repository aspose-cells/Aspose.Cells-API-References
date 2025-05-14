---
title: Validation.Copy
second_title: Aspose.Cells for .NET API Reference
description: Validation method. Copy validation
type: docs
url: /net/aspose.cells/validation/copy/
---
## Validation.Copy method

Copy validation.

```csharp
public void Copy(Validation source, CopyOptions copyOption)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Validation | The source validation. |
| copyOption | CopyOptions | The copy option. |

### Examples

```csharp
// Called: newValidation.Copy(oldValidation, null);
public void Validation_Method_Copy()
{
    Workbook book = new Workbook(Constants.sourcePath + "example.xlsx");
    //Workbook book = new Workbook(path + "Book1.xlsx"); 
    Workbook newWb = new Workbook();
    Worksheet oldWs = book.Worksheets[0];
    Worksheet newWs = newWb.Worksheets[0];

    ValidationCollection oldValidationCollection = oldWs.Validations;
    ValidationCollection newValidationCollection = newWs.Validations;
    int vCount = oldValidationCollection.Count;

    for (int i = 0; i < vCount; i++)
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

    for (int r = 0; r <= maxRow; r++)
    {
        for (int c = 0; c <= maxCol; c++)
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
    //newWb.Save(Constants.destPath + "example.xlsx", SaveFormat.Xlsx);
}
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


