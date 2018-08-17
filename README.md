# Validator

The idea is validate forms easier without missing the flexibility.

So first we import the module and call validator method, like below:

```
import serializar from 'form-serialize';
import Validator from 'validator';

...

submit(e){
    e.preventDefault();

    const formData = serialize(e.target, {hash: true});

    Validator.email(formData)
        && //Do something
}

...
```
