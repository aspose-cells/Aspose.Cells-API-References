---
title: CopyOptions.CopyInvalidFormulasAsValues
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. If the formula is not valid for the dest destination only copy values
type: docs
url: /net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

If the formula is not valid for the dest destination, only copy values.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### Examples

```csharp
// Called: copyOptions.CopyInvalidFormulasAsValues = true;
[Test]
        public void Property_CopyInvalidFormulasAsValues()
        {
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto)
            {
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All)
            };

            Workbook wbSource = new Workbook(Constants.sourcePath + &quot;CellsNet48217.xlsb&quot;, loadOptions);
            Workbook wbDestination = new Workbook(Constants.sourcePath + &quot;CellsNet48217Destination.xlsb&quot;, loadOptions);

            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            foreach (Worksheet wsSource in wbSource.Worksheets)
            {
                Worksheet wsDestination = wbDestination.Worksheets[wsSource.Name];
                if (wsDestination == null)
                {
                    wbDestination.Worksheets.Add(wsSource.Name);
                    wsDestination = wbDestination.Worksheets[wsSource.Name];
                }
                //wsDestination.Copy(wsSource);
                //wbDestination.VbaProject.Modules.Add(wsSource);
            }

            for (int i = 0; i &lt; wbDestination.Worksheets.Count; i++)
            {
                Worksheet wsSource = wbSource.Worksheets[i];
                Worksheet wsDestination = wbDestination.Worksheets[wsSource.Name];

                wsDestination.Copy(wsSource);
                // break;
                //wbDestination.VbaProject.Modules.Add(wsSource);
            }
            wbDestination.CalculateFormula();
            Util.ReSave(wbDestination, SaveFormat.Xlsb);
            //wbDestination.Save(Constants.destPath + &quot;CellsNet48217.xlsb&quot;);
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


