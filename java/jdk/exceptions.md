# Exceptions


ref : [Exceptions: I’m Telling You for the Last Time](https://www.youtube.com/watch?v=rJ-Ihh7RNao)
Eliotte Rusty Harold


## CheckedExceptions
* usecase = pour tout ce qui vient de  _l'environnement exterieur_  à l'application.

Force le dev à prendre en *soin* de ce qui peut mal se passer:
	
	* file I/O
	* encoding
	* OOM
	* ...
	
## RuntimeExceptions
* pour toutes les erreurs de  __dev__

<div class="alert alert-info">
  <i class="fas fa-info-circle"></i> <strong>Note:</strong> 
  Ne pas ajouter de try/catch mais corriger ce type de bug
</div>


## Edge case 

IllegalArgumentException

Exception runtime
mais erreur sur les valeurs qui viennent de l'_exterieur_ (nombre saisie dans une String par exemple)

## try/catch bonnes pratiques

Faire les plus gros blocs possible puis gérer les erreur dans différents catchs

si on log dans les catch, il faut surveiller les logs