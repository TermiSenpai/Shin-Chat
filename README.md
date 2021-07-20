instrucciones para montar la aplicacion sobre electron:

0.- Tener node
1.- sobre la carpeta(vacia) donde estaran los archivos del proyecto:
	npm init
	
2.- Copiar los ficheros del repositorio a la carpeta

3.- npm start

4.- empaquetar y distribuir (TODO y TEST)
	esto está todavia sin probar, pero se supone que va así
	
	añadir dependencias a la app para configurar el andamiaje de Forge
	
	npm install --save-dev @electron-forge/cli
	npx electron-forge import
	
	crear instruccion del make de Forge
	npm run make

	> my-electron-app@1.0.0 make /my-electron-app
	> electron-forge make
	
	Electron Forge crea el fichero de salida con el paquete:
	// Example for macOS
	out/
	├── out/make/zip/darwin/x64/my-electron-app-darwin-x64-1.0.0.zip
	├── ...
	└── out/my-electron-app-darwin-x64/my-electron-app.app/Contents/MacOS/my-electron-app
