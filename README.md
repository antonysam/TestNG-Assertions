# TestNG-Assertions

Assert is defined for verifying wheather the test script gets passed or failed

# Types
1. Hard Assert (will stop the execution)
2. Soft Assert (

_Hard Assert_
```
Assert.assertEquals(<"actual">,<"expected">,"<"Failure reason description">");
Assert.assertTrue(<"value">, "<"Failure description">");
Assert.assertFalse(<"value">)

```

_Soft Assert_

1. If any validation fails it will continue the rest of the script and once scripts completes then it fails the test.

2. when a single validation fails script will be failed at last but the execution will not stop.

3. It is mandatory to call assertAll() method at last. 

```
SoftAssert assertion = new SoftAssert();
assertion.assertEquals(<"actual">,<"expected">);
assertion.assertAll();
```


