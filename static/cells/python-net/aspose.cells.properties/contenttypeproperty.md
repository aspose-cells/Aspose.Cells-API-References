##ContentTypeProperty class
## ContentTypeProperty class
Represents identifier information.
The ContentTypeProperty type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [name](/cells/python-net/aspose.cells.properties/contenttypeproperty/name) | Returns or sets the name of the object. |
| [value](/cells/python-net/aspose.cells.properties/contenttypeproperty/value) | Returns or sets the value of the content type property. |
| [type](/cells/python-net/aspose.cells.properties/contenttypeproperty/type) | Gets and sets the type of the property. |
| [is_nillable](/cells/python-net/aspose.cells.properties/contenttypeproperty/is_nillable) | Indicates whether the value could be empty. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")
```
### See Also
* module [`aspose.cells.properties`](..)
