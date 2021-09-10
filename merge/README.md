### Hacer cambios locales utilizando ramas

`main` = `master` (nueva nomenclatura de github)

### Ejercicios

Crea dos commits en una rama llamada `feature1`


Mergea la rama `feature1` en `main` (a la hora de mergear, no utilizar fast-forward para poder ver como se "unen" las ramas. Nos debería quedar algo de este tipo: 


![explain_git_with_d3](https://cloud.githubusercontent.com/assets/7910250/17195018/537c8e8c-5410-11e6-94fd-041a0c865344.png)

Repítelo de nuevo con una nueva rama llamada `feature2` 

![explain_git_with_d3](https://cloud.githubusercontent.com/assets/7910250/17195052/8fcc8b80-5410-11e6-922d-d61173a1cd57.png)


#### Probamos ahora a realizar un merge con fast-forward

Para ello desde `main` crea una nueva rama llamada `feature2` y realiza 2 commits. Nos quedará algo así: 


![explain_git_with_d3](https://cloud.githubusercontent.com/assets/7910250/17195190/47c33676-5411-11e6-93cb-50f904a14f55.png)

Podemos observar que la  rama `main` apunta a una confirmación que ya está en el historial de la rama` feature1`. Esto significa que todas las confirmaciones en la rama `main` ya están en la rama `feature1`.

En este caso cuando realicemos un merge, estaremos haciendo un *fast-forward merge*, lo que significa que simplemente moverá las referencias `main` y `HEAD` para que apunten al commit  al que apunta `feature1`.

![explain_git_with_d3](https://cloud.githubusercontent.com/assets/7910250/17195338/efa3b078-5411-11e6-81dc-6324701433a4.png)
