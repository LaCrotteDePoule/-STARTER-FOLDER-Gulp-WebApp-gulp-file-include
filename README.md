# Notice #

### Installer le starter théme ###

1. Cloner le dépot dans un dossier vide.
1. npm install
1. bower install
1. gulp serve

### Pour créer le dossier dist ###

gulp build (possibilités erreurs)

### Comment utiliser gulp_file_include ###

index.html
```
#!html
<!DOCTYPE html>
<html>
  <body>
  @@include('./view.html')
  @@include('./var.html', {
    "name": "haoxin",
    "age": 12345,
    "socials": {
      "fb": "facebook.com/include",
      "tw": "twitter.com/include"
    }
  })
  </body>
</html>
```

view.html

```
#!html
<h1>view</h1>
```

var.html

```
#!html
<label>@@name</label>
<label>@@age</label>
<strong>@@socials.fb</strong>
<strong>@@socials.tw</strong>

```