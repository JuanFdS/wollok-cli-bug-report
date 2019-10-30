# wollok-cli-bug-report

[Link al issue](https://github.com/uqbar-project/wollok-cli/issues/24)

## Como reproducir el error

Pararse en la raíz del proyecto y correr `wollok test`, debería verse algo como:
```
Validando archivos Wollok...
Procesando
[WARNING] /ruta/al/proyecto/./src/objects.wlk:2:17 WARNING Unused variable
===========================================================
Ejecutando tests...
Procesando
[WARNING] /ruta/al/proyecto/./src/test2EsteRompe.wtest:5:54 WARNING Unused variable
Running all tests from describe suite de tests
ERROR: null
```

Al menos en unix, se puede validar que el código de error fue 0 corriendo `echo $?` luego de haber corrido `wollok test`.
