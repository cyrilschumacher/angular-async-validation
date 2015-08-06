# angular-async-validation
Example of directive that validate an input in asynchronous.

## How it works?
The source code contain one controller and one directive. The first purposes a method for validate a value. This method is asynchronous: it uses the service: ``$q`` for create a object: ``Promise``.
The second asks the controller method for validate the input through the attribute: ``validator``.

When the user enters characters, the directive will execute the controller method. Meanwhile, it give a value: ``$inProgress`` to indicate progress. After execution, a value "custom" provides the result: ``true`` if input is valid or otherwise, ``false``.