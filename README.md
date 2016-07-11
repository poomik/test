```js
var postcss = require("postcss");
var fs = require("fs");
var css = fs.readFileSync("./css/test.css", "utf-8");
postcss([ require('postcss-bem')({
    defaultNamespace: undefined, // пространство имен по умолчанию для использования, ни по умолчанию
    style: 'suit', // suit или bem, suit установлено по умолчанию,
    separators: {
        descendent: '__' // переписывает любой разделитель по умолчанию, для выбранного стиля
    },
    shortcuts: {
        utility: 'util',
        b:"b"
    }
}) ]).process(css).then( function(res) {
    fs.writeFileSync("./css/out.css", res);
});
```
