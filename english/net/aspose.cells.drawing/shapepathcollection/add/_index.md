---
title: ShapePathCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: ShapePathCollection method. Add a creation path
type: docs
url: /net/aspose.cells.drawing/shapepathcollection/add/
---
## ShapePathCollection.Add method

Add a creation path.

```csharp
public int Add()
```

### Return Value

Returns [`ShapePath`](../../shapepath/) object.

### Examples

```csharp
// Called: int pathIndex = shapePaths.Add();
public static void Method_Add()
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

* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


