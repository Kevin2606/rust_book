### Hello_World
1. El punto de entrada de un programa hecho en Rust se da con la funcion llamada "main"
2. El simbolo "!" significa que no es una funcion comun y corriente, sino una macro
que puede llegar a tener un comportamiento distinto a una funcion normal
3. Al compilar el programa, Rust genera un ejecutable y un archivo con extension ".pdb" que contiene informacion de debug para el ejecutable
### Hello_Cargo
1. Cargo es el gestor de paquetes y tambien puede compilar Rust
2. Comandos con Cargo en la terminal:
    - cargo new <nombre_proyecto> : crea un nuevo proyecto
    - cargo build : compila el proyecto
    - cargo run : compila y ejecuta el proyecto
    - cargo check : compila el proyecto sin crear un ejecutable (mas rapido, usualmente se usa para ver si el codigo compila)
    - cargo build --release : compila el proyecto en modo release (mas lento, pero mas optimizado)
3. Cargo crea un archivo llamado "Cargo.toml" que contiene informacion del proyecto
4. Cargo crea un archivo llamado "Cargo.lock" que contiene informacion de las dependencias del proyecto
5. Cargo crea un directorio llamado "target" que contiene los archivos compilados
6. Cargo no supervisa sus archivos de forma predeterminada. Pero puedes utilizar complementos como [cargo-watch](https://crates.io/crates/cargo-watch) para este propósito.