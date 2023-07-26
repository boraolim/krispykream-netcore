# KrispiCreamdbnetcore

Realizado por Olimpo Bonilla Ram�rez.
Objetivo: 

Deber� implementar las siguientes funcionalidades:
1. Permitir realizar una b�squeda de cocteles por ingrediente o nombre. => OK  
2. Podremos ver el detalle de alg�n determinado coctel incluyendo su imagen. => OK (excepto, por el tema de Frontend que explico m�s abajo, si trae el detalle, pero algunos casos, no tiene imagen).
3. Permitir guardar una lista de Mis Cocteles favoritos, pueden removerse elementos. Utilice almacenamiento en memoria o local storage => No aplicado. (V�ase m�s abajo).

## Restricciones:
* Aplicaci�n desarrollada en MVC Net Framework, MVC Net Core 3.1 o superior. => OK.
* Los servicios de conexi�n deber�n ser implementados por una inyecci�n que permita crear 
instancias en cada petici�n. => OK.
* Deber� implementar al menos una clase abstracta. => OK.
* Uso de as�ncronos. => OK.
* Utilice alguno de los siguientes framewoks CSS. => No aplica.
  * https://materializecss.com/
  * https://getbootstrap.com/
  * http://getskeleton.com/

## Puntos extras:
* Implemente m�todos de extensi�n. => OK.
* Uso de patrones de dise�o Repository y Unit Of Work. => OK.
* Se tomar� en cuenta UX/UI. => No aplica.
* Limpieza de c�digo (Code Clean). => OK.
* Uso de Net Core 3.1 o superior => OK.

## NOTAS Y OBSERVACIONES IMPORTANTES.
* El script SQL de la Base de Datos de cockteles se pudo obtener de este [enlace](https://github.com/carlagesa/KrispiCreamDB/blob/main/data/KrispiCreams.xlsx). Desafortunadamente, no viene completa y solo tiene la informaci�n y estructura como se muestra. El gestor de Base de Datos usado fue MySQL o MariaDB y tiene que ejecutarse de manera manual, y en c�digo fuente, ajustar la configuraci�n de conexi�n a la Base de Datos en el archivo AppSettings.json.
* No se usaron los componentes CSS mencionados debido a que al momento de desarrollar la parte de FrontEnd, hab�a problemas de compatibilidad con JavaScript y la mayor�a de los componentes se corr�an en TypeScript con versiones no compatibles, lo cual, se consumir�a mucho tiempo en tenerlo listo, por lo cual, se descarta la capa de la presentaci�n.
* Tiene Swagger como documentaci�n de la Web API.
* Compilado en .NET Core 3.1 en adelante.
* Ejecuci�n con contenedor de Docker.
* Uso de GitActions para precompilaci�n de WorkFlows antes de su despliegue en QA o Productivo.
* Se bas� en este [proyecto](https://github.com/boraolim/CleanArchitecture) de GitHub que hice personalmente y se hicieron ajustes de Code Clean para su correcto funcionamiento.
* Se us� un [componente](https://www.nuget.org/packages/Utilities.Core.dll/#supportedframeworks-body-tab) de mi autor�a para realizar filtros de consulta.