##TxtLoadStyleStrategy
Specifies how to apply style for parsed values when converting string value to number or datetime.
## TxtLoadStyleStrategy enumeration
Specifies how to apply style for parsed values when converting string value to number or datetime.
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Does not set style for the parsed value. |
| BuiltIn | `1` | Set the style as built-in number/datetime when the parsed value are plain numeric/datetime values. |
| ExactFormat | `2` | Set the exact custom format for the parsed value to make the formatted value be same with the original input one. |
