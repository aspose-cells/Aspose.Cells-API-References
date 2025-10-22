##ExternalLink class
## ExternalLink class
Represents an external link in a workbook.
The ExternalLink type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [type](/cells/python-net/aspose.cells/externallink/type) | Gets the type of external link. |
| [path_type](/cells/python-net/aspose.cells/externallink/path_type) | Get the path type of this external link |
| [original_data_source](/cells/python-net/aspose.cells/externallink/original_data_source) | Represents stored data source of the external link. |
| [data_source](/cells/python-net/aspose.cells/externallink/data_source) | Represents data source of the external link. |
| [is_referred](/cells/python-net/aspose.cells/externallink/is_referred) | Indicates whether this external link is referenced by others. |
| [is_visible](/cells/python-net/aspose.cells/externallink/is_visible) | Indicates whether this external link is visible in MS Excel. |
### Methods
| Method | Description |
| :- | :- |
| [`add_external_name(self, text, refer_to)`](/cells/python-net/aspose.cells/externallink/add_external_name/#system.string-system.string) | Adds an external name. |
### Example
```python
from aspose.cells import Workbook
# Open a file with external links
workbook = Workbook("book1.xls")
# Get External Link
externalLink = workbook.worksheets.external_links[0]
# Change External Link's Data Source
externalLink.data_source = "d:\\link.xls"
```
### See Also
* module [`aspose.cells`](..)
