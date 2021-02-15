# Validatorless

This package provides a means to validate text inputs on the flutter and was inspired by Yup

[Validatorless in pub.dev](https://pub.dev/packages/validatorless)

### how to use

```
dependencies:
  validatorless:
```

```
TextFormField(
  decoration: InputDecoration(
    labelText: 'User e-mail',
  ),
  validator: Validatorless.multiple([
     Validatorless.email('The field must be an email')
     Validatorless.required('The field is obligatory')
   ]),
)
```

### Validatorless functions 

```sh
 Validatorless.required(String)
 Validatorless.email(String)
 Validatorless.min(Number, String)
 Validatorless.max(Number, String)
 Validatorless.number(String) 
```