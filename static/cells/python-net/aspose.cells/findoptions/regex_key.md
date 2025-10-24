##regex_key property
## regex_key property
Indicates whether the searched key is regex.
If true the searched key will be taken as regex and parsed.
Otherwise the key will be parsed according to the rules in ms excel.
### Remarks
Even though the search key has been specified as regex,
it may be refactored according to specified [`FindOptions.look_at_type`](/cells/python-net/aspose.cells/findoptions#look_at_type).
For example, when the type is [`LookAtType.CONTAINS`](/cells/python-net/aspose.cells/lookattype#CONTAINS)(this is the default value for this options),
wildcards will be added at the beginning and end of the search key automatically to ensure the match will be
checked as "contains". In this case, the regular expressions will become more complex
and the performance will also decrease.
So, for performance consideration, if user has specified the exact rule for the regex, then there is no need to
use [`FindOptions.look_at_type`](/cells/python-net/aspose.cells/findoptions#look_at_type) as additional constraint and user may set it as [`LookAtType.ENTIRE_CONTENT`](/cells/python-net/aspose.cells/lookattype#ENTIRE_CONTENT)
to get better performance.
### Definition:
```python
@property
def regex_key(self):
...
@regex_key.setter
def regex_key(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`FindOptions`](/cells/python-net/aspose.cells/findoptions)
