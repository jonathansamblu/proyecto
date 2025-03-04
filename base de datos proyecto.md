CREATE DATABASE TiendaRopa;

USE TiendaRopa;

CREATE TABLE productos (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nombre VARCHAR(255) NOT NULL,
    descripcion TEXT,
    precio DECIMAL(10,2) NOT NULL,
    categoria ENUM('zapatos', 'vestidos', 'accesorios') NOT NULL,
    talla VARCHAR(50),
    color VARCHAR(50),
    stock INT DEFAULT 0,
    imagen_url VARCHAR(255)
);
