---
title: HtmlTableLoadOptionCollection.TableToListObject
second_title: Aspose.Cells for .NET API Reference
description: HtmlTableLoadOptionCollection property. Indicates whether generate list objects from imported tables. The default value is false
type: docs
url: /net/aspose.cells/htmltableloadoptioncollection/tabletolistobject/
---
## HtmlTableLoadOptionCollection.TableToListObject property

Indicates whether generate list objects from imported tables. The default value is false.

```csharp
public bool TableToListObject { get; set; }
```

### Examples

```csharp
// Called: tableLoadOptions.TableToListObject = true;
public static void Property_TableToListObject()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();

            // Create HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Access the HtmlTableLoadOptionCollection instance
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Set the TableToListObject property
            tableLoadOptions.TableToListObject = true;

            // Add a new HtmlTableLoadOption by table index
            int index1 = tableLoadOptions.Add(0);

            // Add a new HtmlTableLoadOption by table id
            int index2 = tableLoadOptions.Add("tableId");

            // Add a new HtmlTableLoadOption by table index and target sheet index
            int index3 = tableLoadOptions.Add(1, 1);

            // Add a new HtmlTableLoadOption by table id and target sheet index
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Add a new HtmlTableLoadOption by table index, target sheet index, and original sheet index
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Add a new HtmlTableLoadOption by table id, target sheet index, and original sheet index
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Access the HtmlTableLoadOption at a specific index
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Set properties of the HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Load an HTML file into the workbook using the load options
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Save the workbook
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


