ALAN KAY UN CAPO
AGUANTE SMALLTALK
CHUPALA C++

historia zzz
![[Pasted image 20250430193320.png]]

no hay una sola forma de hacer el analisis de diseño de objetos sino que hay multiples propuestas 

BOOCH

beneficios de la OO
	1. reusabilidad de software
	2. mejora mantenabilidad y modificabilidad de SW
	3. disminucion de la brecha semantica. representacion consistente en todo el ciclo de vida
	4. mejor interaccion usuario - analista - diseñador
	5. mas apropiado para resolver problemas complejos ([[GUI]], [[Patrones|patterns]], etc)


QUE ES UN SISTEMA OO
	Es un sistema donde sus elementos son entidades a las que denominaremos **objetos**
	que interactuan entre si por medio del envio y recepcion de **mensajes** a esto se le denomina **colaboracion**
	todo esto con el fin de cumplir un objetivo claro y defninido para el sistema
	cada objeto colabora con otro objeto
	cada objeto realiza tareas segun su rol respecto a su **responsabilidad** asignada

concepto d e objeto
	1. un objeto es algo real o abstracto acerca del cual almacenamos datos y operaciones q manipulan dichos datos
	2. **un objeto es una entidad que tiene estado, comportamiento e identidad. La estructura y el comportamiento e  identidad. La estructura y el comportamiento de objetos similares se definen en su clase comun. los terminos instancia y objeto son intercambiables** (booch)

un objeto conoce informacion, realiza servicios, mantiene conecciones (gaona pregunto algo de esto), toma decisiones. Puede ser algo fisico, abstracto, algo del dominio del problema o la solucion


MENSAJE
Los mensajes son el mecanismo por medio del cual se comunican los objetos para poder interactuar y colaborar unos con otros.
emisor---mensaje-->receptor
un mensaje se puede enviar mensajes a un objeto con diferentes propositos

Tipos de mensaje

sincronicos
	se queda plantado esperando la respuesta
asincronicos
	envia mensajes y hace otra cosas mientras espera el callback
de tiempo limite
	combinacion de ambos anteriores, envia la solicitud, hace otra cosa hasta cierta cantidad de tiempo



USABILIDAD
	[[UML]] define responsabilidad como "un contrato u obligacion de un clasificador"
	son cosas que un objeto " ahce" o "conoce" (Larman)
	Hacer:
		hacer algo en si mismo como crear algo o hacer un calculo
		inciar una accion en otros objetos
		controlar y coorrd actividades en otros objetos
	conocer
		concoer datos privados encapsulados
		saber sobre objetos relacionados
		saber sobre cosas que puede derivar o calcular

RESPONSABILIDAD
	Rol es un conjunto relacionado de responsabilidades que puede usarse de manera intercambiable. sinonimo de proposito
	estereotipos de roles
		caracterizacion de las funciones q necesita la app
		al simplifac
		information holder
		structurer
		service provider
		coordinator
		controller
		interfacer

COLABORACION
	una colaboracion se produce cuando dos o mas objetos interactuan entre si para realziar na tarea
	ya que un solo objeto no puede realizar todas las tareas del sistema, deben distribuires en distintos obj
	esta interaccion se hace con mensajes

CONCEPTO DE CLASE
	dos conceptos

	Por una parte conceptualmente una clase es un grupo de objetos con propiedades similares, comportamiento comun, relaciones comunes entre objetos y semantica comun. en ese sentido una clase es un poderoso mecanismo coneptual para agrupar objetos similares en conceptos finitos
	representa conocimiento

	por otra parte una clase es una matriz, un molde que se utiliza
ambas son validas

modelo de objetos (quiere que veamos del libro)
- Abraction
-  encapsulameiento
- herencia 
- y polimorfismo
pero segun booch: 
- abstraccion 
- encapsulamiento 
- modularidad 
- y jerarquia
tres elementos menores
- tipado
- concurrencia
- y persistencia



ABSTRACCION
- proceso mental
- abordar la complejidad
- decidir q es importante y descartar aquello q no lo es
- no es exclusiva de la Orientacion a objetos (OO)
	- aLGORTIMO
	- oBJETO/clase
una abstraccion
	- denota las caracteriticas esenciales de un objeto q lo distinguen de todos los demas tipos de objetos, y por lo tanto proporcionan limites conceptuales claramente definidos, en realacion con la perspectiva del espectador
	- se enfoca en la vista externa de un objeto y asi sirve para separar el comportamiento esencial de unobjeto de su implementacion


perspectiva de una *persona*
personal de universidad -> alumno
mdeicos en un hospital -> paciente


abstraccion de entidad
	los boejtos dasocidadoes a coneptos utiles del dominico o de la solucion son las meores abstrac
abstraccion casual
	un objeto formado por un conjunto de metodos no relacionadps es un ejemplo de mala abstraccion
la abstraccion de un objeto debe preceder a las decisiones de su implementacion 


ENCAPSULAMIENTO
	Es el proceso de compartimentar los elementos de una abstraccion que constituyen sus etrcuture y comportamiento
	sirve para separra la interfaz contractual de una abtracion y su implementacion
	se complementa con la abstraccion
		abstraccion -> comportamiento boservable
		encapsulamiento-> implementacion de ese comportamiento
	empaqueta
		datos
		funciones
	porque se necesita
		control de complejidad
		mantenimiento

muy relacionado con ocultamiento de informacion
	aaaaaaaaaaaaaaaaaaa diapositiva


MODULARIDAD
modularizacion
		dividir un programa en modulso que se pueden compilar por separado pero que tienen conexiones en otros modulos
los leng suelen presentar un constructo similar al de modulo
se colocan estas abstracciones en modulos para producir la arquitectura fiscia del sistema
cuando pensamos en modulos pensamos en aquitectura del sistema
modularidad es la proidedad de un sistema que se ha descompuesto en un conjunto de modulos cohesivos y debilmente acoplados

objetivos:
- reducir costso permitiendo el diseño y la revision dindep
- reducir complejidad
-  AAAAAAAAAAAAAla concha de tu madre gaon me falto est


JERARQUIA(HERENCIA, PARTE DE, AGREGACION)
ES UNA CALSIFICACION U RODENACION DE ABSTRACCIONES
un conjunto de abstracciones a menudo forma una jerarquia
ayudan a simplificar la comprension del problema

jerarquia de clases(herencia)
jerarquia de objetos (composicion)

tipos de herencia: simple o multiple

superclases y subclases


herencia y encapsulamiento
 encapsulamiento: trata de mantener la implementacion oculta exponiendo interfaces
 herencia: comparte las cosas en verdad

privadas -> propia clase
protrgidas -> propia y subclases
publicas -> todos


jERARQUIA DE AGREGACION

es una relacion jerarquica
se representa con el rombo VACIO


DESEABLES
TIPADO
En OO el tipo es igual a una clase
yo siento q no necesito esto asi q no anoto

POLIMORFISMO
	que una variable pueda ser del tipo de sus hijos 
	un operacion puede resolverse de la distinta forma depende de quien la reciba

SOBRECARGA
	definir mas d eun metodo por cada mensaje, los tipos de  los argumentos ayudana decidir a que mensaje se invoca


DISEÑO ORIENTADO A OBJETOS segun booch
- descompsocicion orientada a objetos es la diferencia central con el diseño estructurado (clases vs algortimo)
- "es un metodo de diseño que abarca el proceso de descomposicion orientada a obejt y una notacion etc etc"


FASE EXPLORATORIA INICIAL DE OBJETOS
identificar:
1. clases
	
	- conocimiento gral del dominio del problema
	- sistemas anteriores similares
	- modelos de negocio q puedan analizarse y que esten en relacion con el dominio bajo estudio
	- sesiones de [[tarjetas CRC]]
	- glosarios de terminos
	- Analisis gramatical de enunciado del dominio del problema <- esta es  la q mas se usa en clase en gral

Identificar clases:
- Elegir nombres de class cuidadosamente
- describir su proposito

2. responsabilidades
	Identificar resp
	- para las clases deben determinarse sus responsabilidades
	- encontrar responsabilidades(gralmente verbos), pueden proceder de distintas fuentes(CUs requerimientos adicionales, proposito de clases)
	- algunas opciones son
		- identificar las reponsabilidades del sistema declaras o impl en los Cu
		- cubrir los huecos en los CU y otras descripciones del sistema con resp adicionales a nivel inferior
		- ident responsabilidades para apoyar las relaciones y dependencia entre los candidtaos
	ejercicio "rapido":
		a q obj le corresponden las responsabilidades
			1. contener objetos sin que se ccaigan(taza, tapper  )
			2. soportar el peso de cosas
			3. etc
			4. etc
			5. etc
			6. era la mochila
	- las resp 
	- NO COPIE ESTO POR HACER MEMES
3. colaboraciones
	- las clases pueden cumplir sus resp realizando las operaciones por si solas o colab con otras clases
	- para encontrar colabs
		- es la clase capaz de cumplir sus resp por si misma?, sino de q otra clase necesita
		- q otra clase neceita utilzar las resp de esta clase
	- las clases q no participan en ninguna colaboracion son sospechosas y normalmente se descartan
	- ((alguien pregunto algo q no se entendio un carajo) colaboraciones dentro y fuera del sistema es posible)
	- 
 

etc etc si no sabes POO anda a leer en otro lado q Gaona es un hdp ()