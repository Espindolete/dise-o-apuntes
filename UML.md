
QUE HAY Q LEER
MANUAL DE REFERENCIA CAP 1 2 Y 3
GUIA DE USUARIO CAP 1 Y 2


AREAS = HAY 4


MODELO CONCEPTUAL

EN QUE SE DIVIDEN LAS COSAS?
ETC ETC

VISTA ESTATICA
	Es la base sobre la que se construyen las otras vistas
		conceptos significativos
	captura la estrucutra de los objetos
		OO unifica datos + comportamiento
	incluye operaciones(solo declaracion)
	incluye clasificadores y relaciones
	incluye elementos organizativos como los paquetes

CLASIFICACION
	Clasificador: es un concepto discreto que describe cosas que tienen identidad, estado, comprotamiento y relaciones(UMLUser)
	Clasificador: es una metaclase abstracta cuyas subclases concretas son usadas para clasificar(describir) un conjunto de instancias que tienen caracteristicas comunes( adapt OMG)
	Tipo de clasificadores:
	1. concepto del sistema: clase interaz
	2. conceptos de comportamiento: caso de uso
	3. cosas dle entorno: actor
	4. estructuras de implementacion:componente, nodo, subsistema
==¿¿¿¿Todo clasificador es una clase pero no toda clase es un clasificador dijo????

CLASES & OBJETOS
- Clase: representa un concepto discreto etc etc
- objetos: etc etc
==copiar de la diapo

CLASES: NOTACION GRAFICA
	Cada clase se representa con un rectangulo con 3 "compartimientos"
		1. nombre
		2. atributos
		3. operaciones
		==4. (responsabilidades) no se pq puso esto


RELACIONES
	Las relaciones entre clasificadores son:
		1. asociacion
		2. generalizacion
		3. dependencia
			- uso
			- realizacion
	
Asociacion
		conexion semantica entre instancia de clases
		relacion estructural entre instancias
		proporciona una conexion entre los objetos para le envio de mensajes
		tipicamente binaria
	enlace:
		Instancia de una asociacion
		lista ordenada de referencia a objetos
	Adornos(puede tener):
		- nombre (lo mas importante)
		- rol
		- multiplicidad
		- agregacion/composicion (es una variante de una asociacion, y el adorno q lo marca va sobre la asociacion)
	
	 Nombre:
		Puede tener un nombre en cada direccion(minimo en un sentido)
		puede omitirse en caso de tener nombres del rol
	Rol:
		Es el papel interpretado por una clase en una asociacion
	Multipicidad:
	Agregacion y composicion:
		representa una relacion todo partes entre objetos
		agregacion:
		variante de la asociacion, con mayor fuerza semantica
		Agregacion(o agregacion compartida)
			Pertenencia debil de las partes con el todo
			una parte puede pertenecer a varios todos
			agregacion es siempre * a *
		composicion
			Froma de asociacion mas fuerte en la cual el compuesto es responsabel de gestionar sus partes, por ejemplo, asignacion y designacion
			implica tres cosas
				Dependencia existencial
				hay una partenencia fuerte
				objetos contenidos no son compartidos
			cuando tengo una composicion el rombo significa un 1 en multiplicidad		

Clases: niveles de visibilidad
	- Visibilidad: especifica si el elemento de una calse puede ser usado por otra clase
	- ayuda a definir el nivel de encapsulamiento

GUARDA QUE TEIPO DE DIAGRAMA VAMOS A VER

diagama de clases 😴y objetos 🤨
un diagrama de clases muesra la abstracion de un parte del dominio
un diagramaa de objetos representa una situacion concreta del dominio

![[Pasted image 20250514191749.png]]
nomenclatura del de objetos
	nombre instancia: nombre clase perteneciente

el diagrama tiene objetos (instancais de ??) y enlaces (instancias de asociacion)

Generalizacion:
	Relacion taxnoomica entre una descripcion general y otra mas especifia q la extiende
	relacion "es tipo de"
	relacion ENTRE CLASES
	herencia: mecanismo a traves del cual los atributos operaciones y restricciones definidas para una clase, denom superclase, pueden ser heredados por otras clases subclases
	a veces cuando hay varios niveles de herencia se la dice multinivel

