---
title: ShapePathCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ShapePathCollection property. Gets a creation path
type: docs
url: /net/aspose.cells.drawing/shapepathcollection/item/
---
## ShapePathCollection indexer

Gets a creation path.

```csharp
public ShapePath this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Return Value

Returns [`ShapePath`](../../shapepath/) object.

### Examples

```csharp
// Called: ShapePath newPath = shapePaths[pathIndex];
public static void Property_Int32_()
        {



            // Instantiate a new Workbook
            Workbook workbook = new Workbook(&quot;ShapePathCollectionExample_original.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];

            Shape customShape = worksheet.Shapes[0];
            
            // Access the ShapePathCollection of the arc shape
            ShapePathCollection shapePaths = customShape.Paths;

            if (shapePaths != null)
            {
                // Add a new path to the ShapePathCollection
                int pathIndex = shapePaths.Add();

                // Access the newly added ShapePath
                ShapePath newPath = shapePaths[pathIndex];

                // Display the count of paths in the ShapePathCollection
                Console.WriteLine(&quot;Number of paths in the ShapePathCollection: &quot; + shapePaths.Count);
            }
            

            // Save the workbook
            workbook.Save(&quot;ShapePathCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


