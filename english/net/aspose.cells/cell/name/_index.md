---
title: Cell.Name
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the name of the cell
type: docs
url: /net/aspose.cells/cell/name/
---
## Cell.Name property

Gets the name of the cell.

```csharp
public string Name { get; }
```

### Remarks

A cell name includes its column letter and row number. For example, the name of a cell in row 0 and column 0 is A1.

### Examples

```csharp
// Called: Console.WriteLine($"Cell {cell.Name} has value: {cell.Value} and type: {cell.Type}");
private static void Cell_Property_Name(Cell cell)
        {
            Console.WriteLine($"Cell {cell.Name} has value: {cell.Value} and type: {cell.Type}");

            switch (cell.Type)
            {
                case CellValueType.IsNumeric:
                    Console.WriteLine("The cell contains a numeric value.");
                    break;
                case CellValueType.IsString:
                    Console.WriteLine("The cell contains a string value.");
                    break;
                case CellValueType.IsDateTime:
                    Console.WriteLine("The cell contains a DateTime value.");
                    break;
                case CellValueType.IsBool:
                    Console.WriteLine("The cell contains a boolean value.");
                    break;
                case CellValueType.IsNull:
                    Console.WriteLine("The cell is blank.");
                    break;
                case CellValueType.IsError:
                    Console.WriteLine("The cell contains an error value.");
                    break;
                default:
                    Console.WriteLine("The cell value type is unknown.");
                    break;
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


