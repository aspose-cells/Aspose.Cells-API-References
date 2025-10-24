##custom_function_definition property
## custom_function_definition property
Definition for parsing custom functions.
### Remarks
For some special requirements, such as when calculating custom function in user's custom engine,
some parameters of it need to be caculated in array mode, using this property can mark those parameters
as array mode when parsing the formula. Otherwise user needs to update those custom functions later by
[`Workbook.update_custom_function_definition`](/cells/python-net/aspose.cells/workbook/update_custom_function_definition) to get the same result.
### Definition:
```python
@property
def custom_function_definition(self):
...
@custom_function_definition.setter
def custom_function_definition(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`CustomFunctionDefinition`](/cells/python-net/aspose.cells/customfunctiondefinition)
* class [`FormulaParseOptions`](/cells/python-net/aspose.cells/formulaparseoptions)
