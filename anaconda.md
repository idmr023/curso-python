Ambientes:
	Crear: conda create --name (nombre) [version, si se deja vacío, será la más actual] (archivo)
	Entrar: conda activate (nombre)
	Actualizar nombres: conda create --name (nuevo nombre) --copy --clone (nombre base)
	Desactivar un ambiente: conda deactivate
	Eliminar ambientes: conda env remove --name (nombre)
Librerías:
	Eliminar librerías: conda remove (nombre)
	Instalar: conda install (nombre)
Paquete:
	Instalar desde Anaconda.org: conda install --channel (package owner) (package)
	Enlistar las revisiones del estado del ambiente virtual: conda list --revision
	Volver al estado de una revisión anterior: conda install --revision [nombre_revision]
	Crear una descripción del ambiente solo con los paquetes agregados manualmente (tiene la ventaja que permite mayor compatibilidad multiplataforma, daod que conda se encarga de instalar las dependencias especificas para los paquetes en el SO):
		conda env export --from-history
	Crear un archivo con la descripción(suele ser común en este tipo de archivos el formato .yml):
		conda env export --from-history --file nombre_archivo.yml
	Instalar ambiente virtual desde archivo: conda env create --file nombre_archivo.yml
