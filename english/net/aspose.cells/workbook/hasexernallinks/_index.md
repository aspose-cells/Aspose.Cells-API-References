---
title: Workbook.HasExernalLinks
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Indicates whether this workbook contains external links to other data sources
type: docs
url: /net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Indicates whether this workbook contains external links to other data sources.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Return Value

Whether this workbook contains external links to other data sources.

### Remarks

NOTE: This member is now obsolete. Instead, please use ExternalLinkCollection.Count to check whether there are external links in this workbook. This method will be removed 12 months later since December 2021. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: var b1 = userWorkbook.HasExernalLinks();
[Test]
        public void Method_HasExernalLinks()
        {
            string genericTemplatePath = Constants.sourcePath + &quot;CelsNet402901.xlsm&quot;;

            string externalLinkFilePath = Constants.sourcePath + &quot;CelsNet402902.xlsx&quot;;

            Workbook mainWorkbook =  new Workbook(genericTemplatePath);

            Workbook userWorkbook = new Workbook(externalLinkFilePath);

            //This gets rid of the exception but we should not remove all the names

            //currentWorkbook.Worksheets.Names.Clear();

            var b1 = userWorkbook.HasExernalLinks();

            //This does not helps. Furthemore, both b1 and b2 are True...

            userWorkbook.Worksheets.ExternalLinks.Clear(); //userWorkbook.RemoveExternalLinks();

            var b2 = userWorkbook.HasExernalLinks();

            mainWorkbook.Combine(userWorkbook);

            MemoryStream ms = new MemoryStream();

            //This causes the &quot;Object reference not set to an instance of an object.&quot; at Aspose.Cells.ExternalSheetCollection.FindSupbook(Int32 refIndex)...

            mainWorkbook.Save(ms, SaveFormat.Xlsx);

        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


