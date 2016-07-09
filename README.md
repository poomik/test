# test
test

 +@utility blockName {
 +    color: blue;
 +}
 +
 +@utility blockName span {
 +    color: green;
 +}
 +
 +@component elementName {
 +    color: brown;
 +
 +    @modifier mName {
 +        color: greenyellow;
 +    }
 +
 +    @descendent dName {
 +        color: aqua;
 +    }
 +
 +    @when sName {
 +        color: gainsboro;
 +    }
 +}
 +
 +@component-namespace nmsp {
 +    @component ComponentName {
 +        color: red;
 +    }
