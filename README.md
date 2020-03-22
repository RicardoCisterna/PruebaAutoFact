Mejoras a las solucion.

Arquitectura:

1-agregar api rest node,
2-crear base de datos,
usuarios -> permisos 
usurios -> encuestas -> preguntas -> respuestas
preguntas -> tipos_pregunta (esto para poder agregar, multimples encuestas, con distintos tipos de pregunta y a futuro no sea necesario crear una vista por cada tipo de pregunta, y se puedan mostrar de forma automatica)
3- ingreso a usuario por medio de correo google

Seguridad:

-implementar jwt para crear tokens de acceso a la app.
-manejar permisos de usuarios, a nivel de api y web

Esclabilidad:
- con la api rest montada en la nube, que funcione de forma serverless o montada
con un balanceador de carga y que tenga auto escalado automatico (cuidado con los ataques Dos)
- una base de datos, que soporte la cantidad de llamados. 

Rendimiento:


Diseño:
-a nivel de front end, falta definir comportamientos, la forma que se presenta la informacion.
-definir lenguaje (de que manera se muestra la informacion al usuario, si hay segmentacion de usuarios puede que se tenga que mostrar un lenguaje diferente).

Despliegue:

-para la api, tenia considerado desplagarlo en zeit y bd con mongo db,
con ambos se puede desplegar de forma gratuita para realizar pruebas (pre productivas).
-se puede armar un despliegue automático, pero eso por ahora supera mis conocimientos.

Otros:
-Recomendacion, para la prueba tecnica, en 4 horas es muy poco tiempo para realizar una
tarea de este estilo, sobre todo si no se tiene ningun contexto de como va a ser la prueba de antemano.
realizar modelo de bd, pensar como debe verse el fron y como conectar una api con el front. 
solo planear puede tomar más de 4 horas. 





# auto_front

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
