-- Crear la tabla Instructores
CREATE TABLE Instructores (
    instructor_id INT AUTO_INCREMENT PRIMARY KEY,
    nombre VARCHAR(100),
    apellido VARCHAR(100),
    especializacion VARCHAR(100),
    telefono VARCHAR(15)
);

-- Crear la tabla Cursos
CREATE TABLE Cursos (
    curso_id INT AUTO_INCREMENT PRIMARY KEY,
    nombre VARCHAR(100),
    descripcion TEXT,
    fecha_inicio DATE,
    fecha_fin DATE,
    instructor_id INT,
    FOREIGN KEY (instructor_id) REFERENCES Instructores(instructor_id)
);

-- Crear la tabla Estudiantes
CREATE TABLE Estudiantes (
    estudiante_id INT AUTO_INCREMENT PRIMARY KEY,
    nombre VARCHAR(100),
    apellido VARCHAR(100),
    correo VARCHAR(100),
    telefono VARCHAR(15)
);

-- Crear la tabla Inscripciones
CREATE TABLE Inscripciones (
    inscripcion_id INT AUTO_INCREMENT PRIMARY KEY,
    curso_id INT,
    estudiante_id INT,
    fecha_inscripcion DATE,
    FOREIGN KEY (curso_id) REFERENCES Cursos(curso_id),
    FOREIGN KEY (estudiante_id) REFERENCES Estudiantes(estudiante_id)
);

-- Crear la tabla Materiales
CREATE TABLE Materiales (
    material_id INT AUTO_INCREMENT PRIMARY KEY,
    curso_id INT,
    nombre VARCHAR(100),
    tipo VARCHAR(50),
    url VARCHAR(255),
    FOREIGN KEY (curso_id) REFERENCES Cursos(curso_id)
);
