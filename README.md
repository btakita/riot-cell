# riot-cell
riotjs cell programming (aka observers, signals/slots, computed properties)

## Usage

~~~javascript
var cell = require('riot-cell')
  , cat = cell()('Fluffy').send(catOnChange).on('change', catOnChange)
  ;
cat('Pickles')
function catOnChange(cat2) {
  console.log('I love '+cat2+'!');
}
~~~

~~~
I love Fluffy!
I love Pickles!
~~~