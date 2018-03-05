# PracticaGit - Respuestas

### CONTRERAS MORA, ANA
--

**1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

`git reset -- HEAD~1` 

Porque mediante este comando dejamos el working tree sin modificar, pero deshace el commit y deja los cambios que se han commiteado sin procesar, de esta manera nos saldran estos archivos como que tienen cambios no realizados para la confirmación.

--

**2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

`git reflog` 

`git reset --hard "dc3e3f1"`

Con el git reflog vemos el listado de cambios que se han realizado para poder seleccionar el código asociado al commit al que queremos volver.

Con el git reset --hard "dc3e3f1, reseteamos esta rama y todos sus cambios al commit con el codigo especificado en el ultimo parámetro.


--

**3. El merge del paso 13, ¿Causó algún conflicto? ¿Porqué?**

No causa ningún conflicto. Puesto que la rama styled esta creada a partir de la master y la master no contiene ningun cambio que afecte a styled.


--
**4. El merge del paso 19, ¿Causó algún conflicto?¿Porqué?**

Sí, porque los cambios realizados en la rama htmlify cambiaban el mismo archivo que la rama styled.

--
**5. El merge del paso 21, ¿Causó algún conflicto?¿Porqué?**

No causa ningun conflicto, porque en la rama styled el cambio en el archivo don quijote viene desde master y solo se ha cambiado en styled y no en master, es por esto que no hay conflicto en las dos ramas.


--
**6. ¿Qué comando o comandos utilizaste en el paso 25?**

`git log --graph`


--
**7. El merge del paso 26,¿Podría ser fast forward?¿Porqué?**

Si porque title es una rama que sale de master y esto permite hacer un merge con el modo fast forward.

--

**8. ¿Qué comando o comandos utilizaste en el paso 27?**

`git revert "hash del commit del merge"`

--

**9. ¿Qué comando o comandos utilizaste en el paso 28?**

`git reset --hard`

--

**10. ¿Qué comando o comandos utilizaste en el paso 29?**

`git branch -D title`


--

**11.¿Qué comando o comandos utilizaste en el paso 30?**

`git reflog"`

`git reset --hard "numeroDelCommit"`

Lanzamos el comando git reflog para saber el numero de commit donde hicimos el merge del title. Y volvemos a esa version con el git reset.


--

**12.¿Qué comando o comandos usaste en el paso 32?**

`git reflog"`

`git reset --hard "numeroDelCommitInicial"`

Lanzamos el comando git reflog para saber el numero de commit donde hicimos el texto del poema. Y volvemos a esa version con el git reset.

--
**13.¿Qué comando o comandos usaste en el punto 33?**

`git reflog"`

`git reset --hard "numeroDelCommitFinal"`

Lanzamos el comando git reflog para saber el numero de commit donde hicimos el merge del title. Y volvemos a esa version con el git reset.

--
