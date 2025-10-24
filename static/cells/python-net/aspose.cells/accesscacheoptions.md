##AccessCacheOptions enumeration
## AccessCacheOptions enumeration
Cache options for data access. Can be combined with | operator for multiple options together.
The AccessCacheOptions type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| NONE | No cache for any data access. |
| ALL | Apply all possible optimizations for all kinds of data access in the workbook.
| POSITION_AND_SIZE | Apply possible optimization for getting object(such as Shape)'s position and size.
| CELLS_DATA | Apply possible optimization for getting cells' values.
| CELL_DISPLAY | Apply possible optimization for getting display-related results of
| GET_FORMULA | Apply possible optimization for getting formulas.
| SET_FORMULA | Apply possible optimization for setting formulas.
| CALCULATE_FORMULA | Apply possible optimization for calculating formulas.
| CONDITIONAL_FORMATTING | Apply possible optimization for getting formatting result of conditional formattings.
| VALIDATION | Apply possible optimization for getting validation result.
### Remarks
For some features, accessing large dataset requires a lot of repeated and complicated operations
such as search, calculation, ...etc and those operations will take a lot of extra time.
For common situations, all dependent data remains unchanged during the access, so some caches can be built and used to
improve the access performance.
For this purpose, we provide this API so that user can specify which kind of data access needs
to be optimized by possible caching mechanism.
Please note, for different options, different data set may be required to be "read-only".
And performance of accessing data depends on many aspects, the use of caching mechanism
does not guarantee that performance will be improved. For some situations,
such as the dataset to be accessed is small, using cache may cause even more time because
caching itself also needs certain extra time.
### See Also
* module [`aspose.cells`](..)
