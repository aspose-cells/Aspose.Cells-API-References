---
title: OoxmlSaveOptions.LightCellsDataProvider
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. The data provider for saving workbook in light mode
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/lightcellsdataprovider/
---
## OoxmlSaveOptions.LightCellsDataProvider property

The data provider for saving workbook in light mode.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Examples

```csharp
// Called: LightCellsDataProvider = dataProvider
public static void OoxmlSaveOptions_Property_LightCellsDataProvider()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a custom LightCellsDataProvider
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // Set the LightCellsDataProvider for saving the workbook
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Save the workbook with the custom LightCellsDataProvider
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
```

### See Also

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


