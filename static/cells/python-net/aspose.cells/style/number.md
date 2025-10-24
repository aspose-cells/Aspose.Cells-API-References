##number property
## number property
Gets or sets the display format of numbers and dates. The formatting patterns are different for different regions.
### Remarks
For example, the formatting patterns represented by numbers for en_US region:
| Value | Type | Format String |
| :- | :- | :- |
| 0| General |
| 1| Decimal |
| 2| Decimal |
| 3| Decimal |
| 4| Decimal |
| 5| Currency |
| 6| Currency |
| 7| Currency |
| 8| Currency |
| 9| Percentage |
| 10| Percentage |
| 11| Scientific |
| 12| Fraction |
| 13| Fraction |
| 14| Date |
| 15| Date |
| 16| Date |
| 17| Date |
| 18| Time |
| 19| Time |
| 20| Time |
| 21| Time |
| 22| Time |
| 37| Accounting |
| 38| Accounting |
| 39| Accounting |
| 40| Accounting |
| 41| Accounting |
| 42| Currency |
| 43| Accounting |
| 44| Currency |
| 45| Time |
| 46| Time |
| 47| Time |
| 48| Scientific |
| 49| Text |
### Definition:
```python
@property
def number(self):
...
@number.setter
def number(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Style`](/cells/python-net/aspose.cells/style)
