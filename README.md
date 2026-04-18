# Taller-de-programaci-n-
Crear la clase cliente

class Cliente:
    
    Clase que crea objetos de tipo cliente

    def __init__(self, nombre, apellido, genero, ocupacion):
        self.__nombre = nombre
        self.__apellido = apellido
        self.__genero = genero
        self.__ocupacion = ocupacion

    @property
    def nombre(self):
        return self.__nombre

    @nombre.setter
    def nombre(self, nuevo_nombre):
        self.__nombre = nuevo_nombre

    @property
    def apellido(self):
        return self.__apellido

    @apellido.setter
    def apellido(self, nuevo_apellido):
        self.__apellido = nuevo_apellido

    @property
    def genero(self):
        return self.__genero

    @genero.setter
    def genero(self, nuevo_genero):
        self.__genero = nuevo_genero

    @property
    def ocupacion(self):
        return self.__ocupacion

    @ocupacion.setter
    def ocupacion(self, nueva_ocupacion):
        self.__ocupacion = nueva_ocupacion

    def __str__(self):
        return f"Cliente [{self.__dict__}]"

if __name__ == "__main__":
    cliente1 = Cliente("Maria", "Paz", "F", "Estudiante")

    print(cliente1.nombre)

    if cliente1.genero == "M":
        print("Masculino")
    else:
        print("Femenino")

    print(cliente1.ocupacion)
    print(cliente1)
