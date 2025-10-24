##InputMethodEditorMode Enum
'InputMethodEditorMode enum. Encapsulates the object that represents inputmethodeditormode in Go.'
## InputMethodEditorMode Enum
Represents the default run-time mode of the Input Method Editor.
```go
type InputMethodEditorMode int32
```
## Fields
| Field | Description |
| --- | --- |
|[NoControl](./nocontrol/) | Does not control IME. |
|[On](./on/) | IME on. |
|[Off](./off/) | IME off. English mode. |
|[Disable](./disable/) | IME off.User can't turn on IME by keyboard. |
|[Hiragana](./hiragana/) | IME on with Full-width hiragana mode. |
|[Katakana](./katakana/) | IME on with Full-width katakana mode. |
|[KatakanaHalf](./katakanahalf/) | IME on with Half-width katakana mode. |
|[AlphaFull](./alphafull/) | IME on with Full-width Alphanumeric mode. |
|[Alpha](./alpha/) | IME on with Half-width Alphanumeric mode. |
|[HangulFull](./hangulfull/) | IME on with Full-width hangul mode. |
|[Hangul](./hangul/) | IME on with Half-width hangul mode. |
|[HanziFull](./hanzifull/) | IME on with Full-width hanzi mode. |
|[Hanzi](./hanzi/) | IME on with Half-width hanzi mode. |
