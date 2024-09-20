# POO
Clases, Objetos e información relativa a POO en proyecto Biblioteca

Para conectar DB instalamos y usamos XAMPP con Apache y MySQL
https://www.tutorialesprogramacionya.com/pythonya/detalleconcepto.php?punto=81&codigo=81&inicio=75
    Ejecutar en terminal:
        pip install mysql-connector

Para validación de RUT, usamos rut-chile
https://pypi.org/project/rut-chile/
    Ejecutar en terminal:
        pip install rut_chile
    Uso:
        from rut_chile import rut_chile

        rut_chile.is_valid_rut("12345678-9")
        # returns False
        rut_chile.is_valid_rut("6265837-1")
        # returns True

        # Formatos soportados

        rut_chile.is_valid_rut("98685030")
        # returns True
        rut_chile.is_valid_rut("9868503-0")
        # returns True
        rut_chile.is_valid_rut("9.868.503-0")
        # returns True
        rut_chile.is_valid_rut("12.667.869-K")
        # returns True
        rut_chile.is_valid_rut("12.667.869-k")
        # returns True