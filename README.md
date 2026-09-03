# practica2_253239

1. ¿Hizo falta una base de datos real para probar la regla de negocio? ¿Qué dice eso sobre para qué sirve el patrón Repository?
No, la probe completa usando solo una lista en memoria y eso me hizo ver que el patrón Repository sirve justo para eso no importa como se guarden los datos por dentro mientras cumplan lo basico el resto del programa funciona igual.

2. El Service recibe el repositorio como Repository<Prestamo>, no InMemoryPrestamoRepository. ¿Qué se rompía si usaban la clase concreta?
Si mi Service dependiera directo de la clase en memoria pues quedaria amarrado a esa opción y si un día que cambie a una base de datos real pues tendria que modificar el Service tambien

3. Si cambiaran el Map en memoria por una base de datos real, ¿cuántos archivos tocarían? ¿Por qué tan pocos?
diria que pocos solo uno nuevo al repositorio conectado a la base de datos real y una línea en main.ts para pues poder usarlo
