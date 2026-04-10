##git log vs git reflog
git log muestra el historial de commits del proyecto que están en las ramas actuales. Es decir, lo que normalmente se ve del proyecto.

git reflog muestra todos los movimientos que ha hecho HEAD, como commits, cambios de rama o resets, incluso si esos commits ya no aparecen en git log.

##Situación

git reflog puede salvarte si haces un git reset --hard por error o borras una rama importante. Aunque los commits desaparezcan del git log, se pueden encontrar en el reflog y recuperar creando otra rama o volviendo a ese commit.

##Por qué hay que tener ciudado?
Aunque git reflog ayuda a recuperar cosas, no es infinito. Con el tiempo los datos pueden desaparecer.

Por eso hay que tener cuidado con comandos como git reset --hard, porque puedes perder trabajo y no siempre será fácil recuperarlo.
