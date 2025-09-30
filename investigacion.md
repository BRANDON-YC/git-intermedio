PRACTICA # 2
Parte I – Investigación
1 ¿Qué es una rama (branch) en Git y para qué se utiliza?
una línea de trabajo aislada que apunta a un commit y se mueve con tus nuevos commits
Sirve para desarrollar features, corregir bugs, experimentar o preparar releases sin romper main.
2 Explica con tus palabras qué significa hacer un merge.
juntar dos líneas de tiempo dos ramas en una sola, integrando cambios de ambas.
3 ¿Qué es un conflicto de fusión (merge conflict) y cómo se puede resolver?
 Conflicto de fusión = choque de cambios en las mismas líneas/archivos entre ramas
Solución
Abre el archivo y elige versión (tuya/ajena/mixta).
Borra marcadores <<<<<<< ======= >>>>>>>.
git add archivo
Si era merge: git commit · Si era rebase: git rebase --continue (Para salir: git merge --abort / git rebase --abort).
4 Diferencia entre fork y clone en GitHub.
Fork: copia remota de un repo a tu cuenta de GitHub. Útil para contribuir a proyectos donde no tienes permisos.
Clone: copia local de un repo (el original o tu fork) a tu PC.
Fork = copia remota en GitHub; Clone = copia en tu máquina.
5 ¿Qué es un pull request y para qué se usa en proyectos colaborativos?
 solicitud para integrar una rama (o fork) en otra dentro de GitHub. Revisión de código (comentarios, cambios solicitados). Permisos y control (no tocas main sin aprobación).
6 Investiga y explica 3 buenas prácticas para colaborar en equipo usando GitHub.
1_ Ramas pequeñas con Pull Request obligatorio y rama principal protegida.
Exige al menos una o dos revisiones antes de integrar y prohíbe envíos directos a la rama principal mediante reglas protección.
2_ Commits atómicos con mensajes claros y trazables.
Escribe mensajes descriptivos (por ejemplo, estilo Conventional Commits) y en cada Pull Request vincula y cierra la incidencia correspondiente (“Cierra #123”).
3_ Integración Continua y Entrega Continua con comprobaciones obligatorias.
Antes de integrar, exige que pasen las pruebas automatizadas, los analizadores de código (linters), la compilación y que la rama esté actualizada respecto a la rama principal
