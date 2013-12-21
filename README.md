parsii
======

Super fast and simple evaluator for mathematical expressions written in Java

Using it is as simple as:

Scope scope = Scope.create();
Variable a = scope.getVariable("a");
Expression expr = Parser.parse("3 + a * 4");
a.setValue(4);
System.out.println(expr.evaluate());
a.setValue(5);
System.out.println(expr.evaluate());

For your convenience: A pre-built jar can be found in the build directory.