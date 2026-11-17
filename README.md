# BICHOMANIA_PRUEBAS_DE_RENDIMIENTO

Pruebas de rendimiento con JMeter 5.x para el backend.

## Ejecutar

Levantar el backend:

```
cd backend
npm install
npm start
```

Ejecutar el plan desde la raiz del repositorio:

```
jmeter -n -t jmeter/plan_rendimiento.jmx -l jmeter/resultados/aggregate.csv -e -o jmeter/resultados/reporte
```

Usar otro servidor, puerto o producto:

```
jmeter -n -t jmeter/plan_rendimiento.jmx -Jservidor=localhost -Jpuerto=3001 -Jid_producto=1 -l jmeter/resultados/aggregate.csv -e -o jmeter/resultados/reporte
```

El reporte HTML queda en jmeter/resultados/reporte/index.html. Los casos estan descritos en jmeter/casos_de_prueba.md.
