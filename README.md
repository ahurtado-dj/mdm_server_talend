======================================
TALEND MDM
======================================

basa su estructura en la existencia de un hub central de datos definido por talend: por debajo el repositorio es xml llamada "eXist" y ofrece la forma de crear vistas y busquedas
se define al inicio la estructutra de la entidad en un exquema xsd
posteriormente se crean estructuras para entrada o salida. Luego se deben hacer los jobs de exportacion o importacion de datos y existen una especie de listeners que tiene talend para conocer cuando se modifican los registros del repositorio central.
El esquema planteado por talend para MDM no es práctico para el escenario del sistema actual. 

para poder realizar proyectos MDM se 
- instalacion: 
	se descomprime el studio
	se ejecuta el instalador del server
		(usuario: sa/sa)
		
- ejecucion
	subir el mdm_server (tomcat en el cual se instaló el server)
	ir a http://localhost:8180/talendmdm (por defecto el usuario es user/user, admin/talend o administrator/administrator)
	
- diseño
	ir al panel mdm y agregar una nueva conexion
	nombre: talendmdm_server
	user: (admin/talend ) usuario interno para publicar
	ubicacion: 
	
	
	mdm repository (actualizar desde el server)
	-> crear nueva instancia en datamodel
	-> datacontainer debe tener el mismo nombre que el datamodel
	
	
----------------
MODELO de mediacion
	
> conexion a servidor talend_mdm

nombre: MDM_Persona
	Link:
		version: 6.0
		user: admin
		password: talend
		server_url: http://localhost:8180/talendmdm/services/soap


ir a las vistaas del modelo, en: http://localhost:8180/talendmdm





	