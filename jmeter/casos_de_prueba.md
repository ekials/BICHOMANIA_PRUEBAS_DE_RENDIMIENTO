# Casos de prueba de rendimiento

| #TC | Escenario | URL y metodo | % de carga total | Usuarios | Subida | Tiempo aceptable |
|-----|-----------|--------------|------------------|----------|--------|------------------|
| TC1 | Listar productos | GET /productos | 10% | 100 | 10 s | 1000 ms |
| TC2 | Crear producto | POST /productos/agregar | 30% | 300 | 10 s | 3000 ms |
| TC3 | Editar producto | PUT /productos/editar/${id_producto} | 30% | 300 | 10 s | 3000 ms |

Cada grupo de hilos ejecuta una sola iteracion por usuario y usa un Constant Timer de 300 ms.

Variables del plan: servidor (localhost), puerto (3001), id_producto (1).
