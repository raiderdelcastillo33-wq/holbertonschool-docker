# Docker Mistakes

## **`tree`: command not found**

Error:

```
tree -L 2
```

Salida:

```
zsh: command not found: tree
```

Solución:

```
find . -maxdepth 2 -type d | sort
```

Lección:

No asumir que una herramienta está instalada.

---

## **Usar nombres genéricos en comandos**

Error:

```
cat archivo
cat archivo_real
```

Salida:

```
cat: archivo: No such file or directory
cat: archivo_real: No such file or directory
```

Solución:

Usar siempre rutas reales:

```
cat notes/docker-cheatsheet.md
cat notes/docker-concepts-summary.md
cat notes/mistakes.md
```

Lección:

En el flujo real Holberton no se usan marcadores genéricos. Se usan rutas exactas.

---

## **Archivo creado en la carpeta equivocada**

Error:

```
notes/examples/docker-concepts-summary.md
```

Solución:

```
mv notes/examples/docker-concepts-summary.md notes/docker-concepts-summary.md
```

Verificación:

```
find notes -type f | sort
```

Lección:

Verificar la estructura antes de hacer commit.

---

## **Git muestra `Untracked files`**

Salida:

```
Untracked files:
    notes/
```

Significado:

Git ve archivos nuevos, pero todavía no los está siguiendo.

Solución:

```
git add notes
git status
```

Lección:

`Untracked files` no es un error. Es una señal de archivos nuevos pendientes de añadir.
