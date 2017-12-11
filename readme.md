# are-intervals-overlapping

> Check if two intervals are overlapping - Logic from date-fns

## Install ##

    npm install --save are-intervals-overlapping

or

    yarn add are-intervals-overlapping


## Usage ##

```js
var areIntervalsOverlappings = require('are-intervals-overlapping');
// or
import areIntervalsOverlappings from 'are-intervals-overlapping';

// For overlapping time intervals:
areIntervalsOverlapping(
  {start: new Date(2014, 0, 10), end: new Date(2014, 0, 20)},
  {start: new Date(2014, 0, 17), end: new Date(2014, 0, 21)}
)
//=> true

// For non-overlapping time intervals:
areIntervalsOverlapping(
  {start: new Date(2014, 0, 10), end: new Date(2014, 0, 20)},
  {start: new Date(2014, 0, 21), end: new Date(2014, 0, 22)}
)
//=> false

// Using the inclusive option:
areIntervalsOverlapping(
  {start: new Date(2014, 0, 10), end: new Date(2014, 0, 20)},
  {start: new Date(2014, 0, 20), end: new Date(2014, 0, 24)}
)
//=> false

areIntervalsOverlapping(
  {start: new Date(2014, 0, 10), end: new Date(2014, 0, 20)},
  {start: new Date(2014, 0, 20), end: new Date(2014, 0, 24)},
  {inclusive: true}
)
//=> true
```

## License ##

MIT © [Diego Jara](saintplay96@gmail.com)
