======================================
TALEND MDM
======================================

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





	