---
title: WorkbookSettings.DisplayDrawingObjects
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Indicates whether and how to show objects in the workbook
type: docs
url: /net/aspose.cells/workbooksettings/displaydrawingobjects/
---
## WorkbookSettings.DisplayDrawingObjects property

Indicates whether and how to show objects in the workbook.

```csharp
public DisplayDrawingObjects DisplayDrawingObjects { get; set; }
```

### Examples

```csharp
// Called: settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;
public static void Property_DisplayDrawingObjects()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the workbook settings
            WorkbookSettings settings = workbook.Settings;

            // Set the DisplayDrawingObjects property to show all objects
            settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;

            // Save the workbook
            workbook.Save(&quot;DisplayDrawingObjectsExample_DisplayShapes.xlsx&quot;);

            // Set the DisplayDrawingObjects property to show placeholders
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Placeholders;

            // Save the workbook
            workbook.Save(&quot;DisplayDrawingObjectsExample_Placeholders.xlsx&quot;);

            // Set the DisplayDrawingObjects property to hide all shapes
            settings.DisplayDrawingObjects = DisplayDrawingObjects.Hide;

            // Save the workbook
            workbook.Save(&quot;DisplayDrawingObjectsExample_Hide.xlsx&quot;);
            workbook.Save(&quot;DisplayDrawingObjectsExample_Hide.pdf&quot;);
            return;
        }
```

### See Also

* enum [DisplayDrawingObjects](../../displaydrawingobjects/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


