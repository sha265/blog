# How to set a conditional breakpoint on exception in Chrome

If you know that a certain part of your javascript code triggers an exception, you can use the following code to evaluate your exception as a boolean expression by Chrome:

```
try{ json_parse(input); true } catch(x) { false }
```

For example, in this case, I had a specific value of the `input` that was causing `json_parse()` to throw an exception, and I only wanted the browser to break on this specific value.

To set a conditional breakpoint in chrome:
https://developers.google.com/web/updates/2015/07/set-a-breakpoint-based-on-a-certain-condition