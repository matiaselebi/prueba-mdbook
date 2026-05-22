# prueba-mdbook

debemos tener instalado rust, mdBook y c++ (desde visual studio: MSVC v143 o v142 Windows 10/11 SDK C++ CMake tools, si aparece)
una vez teniendo instalado rust y las librerias de c++, para instalar mdbook necesitamos descargar el archivo de github y desde la carpeta abrir un cmd y poner este comando cargo install mdbook para instalar mdbook

para crear un libro necesitamos crear una carpetra mediante ese comando: mdbook init my-first-book, para correr el mdbook tenemos que poner este codigo: mdbook serve --open

para exportarlo en pdf se necesita instalar esta extension mediante la terminal de visual studio code: cargo install mdbook-pdf.
En book.toml poner este codigo:
[output.html]
print = { enable = true }

[output.pdf].
Para exportarlo como PDF en la terminal del libro que queres exportar pones este codigo: mdbook build
