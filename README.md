# TM-312

We are aiming to convert roman numerals to binary. We want to start my recognizing is a roman numeral is valid.


## Rules

| Numeral| Value |
|---------|-------|
| I       |   1   |
| V       |   5   |
| X       |   10  |
| L       |   50  |
| C       |   100 |
| D       |   500 |
| M       |   1000|

### Additivity
- When a numeral is followed by one of equal or lesser value you add
  - VI = 5 + 1 = 6
### Subtractivity
- When a numeral is followed by one of greater value you subtract
  - IV = 5 - 1 = 4
- V, L, D **cannot** subtract
  - [Wrong] - VC
- Subtraction must happen between within two numeral levels
  - [Valid] - XC
  - [Wrong] - XD 
### Repitition
- A numeral can only repeat up to **3** times
  - III = 3
  - [Wrong] - IIII
- V, L, D should **never** be repeated
 
