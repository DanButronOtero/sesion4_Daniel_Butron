# Sesion 4

## Reto 1



### Fecha, nombre y texto de cada comentario.

```json
{
    date:1,
    name:1,
    text:1
}
```



![1](img/1.png)

### Título, elenco y año de cada película.

```json
{
    title:1,
    cast:1,
    year:1
}
```

![2](img/2.png)

### Nombre y contraseña de cada usuario.

```json
{
    name:1,
    password:1
}
```

![3](img/3.png)





## Reto 2

### ¿Qué comentarios ha hecho Greg Powell?

```json
{name:"Greg Powell"}
```

![4](img/4.png)

### ¿Qué comentarios han hecho Greg Powell o Mercedes Tyler?

```json
{
    $or:[
        {name:"Greg Powell"},
        {name:"Mercedes Tyler"}
    ]
}
```



![5](img/5.png)

### ¿Cuál es el máximo número de comentarios en una película?

```json
{
 project: {
  title: 1,
  num_mflix_comments: 1
 },
 sort: {
  num_mflix_comments: -1
 },
 limit: 1
}
```

![6](img/6.png)



### ¿Cuál es título de las cinco películas más comentadas?

```json
{
 project: {
  title: 1,
  _id: 0
 },
 sort: {
  num_mflix_comments: -1
 },
 limit: 5
}
```

![7](img/7.png)