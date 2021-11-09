# Date Range Picker

This date range picker component creates a dropdown menu from which a user can
select a range of dates.

This is a fork of "dangrossman/daterangepicker" plugin. For complete documentation please refer, https://github.com/dangrossman/daterangepicker and http://www.daterangepicker.com

### Features

- Removed the Moment.js dependency and replaced it with Day.js (https://day.js.org/).



#### Usage

```
npm i daterangepicker-dayjs
```


##### How to use
```javascript
import $ from "jquery";
import dayjs from "dayjs";
import "daterangepicker-dayjs/daterangepicker";
import "daterangepicker-dayjs/daterangepicker.css";

// Plugins
import localeData from "dayjs/plugin/localeData";
import localizedFormat from "dayjs/plugin/localizedFormat";
import isoWeek from "dayjs/plugin/isoWeek";
import arraySupport from "dayjs/plugin/arraySupport";
import badMutable from "dayjs/plugin/badMutable";

// Load plugins
dayjs.extend(localeData);
dayjs.extend(localizedFormat);
dayjs.extend(isoWeek);
dayjs.extend(arraySupport);
dayjs.extend(badMutable);

// Simple Date Range Picker
$('input[name="dates"]').daterangepicker();
```

##### HTML 

```html
<div>
	<h3>Simple Date Range Picker</h3>
	<input type="text" name="dates" class="form-control pull-right" />
</div>
```



## License

The MIT License (MIT)

Copyright (c) 2012-2020 Dan Grossman

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
