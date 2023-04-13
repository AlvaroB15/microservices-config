```yaml

# ESTE ES LA CONFIGURACION MAS GENERAL, ADEMAS DE AGREGAR EL PUERTO RANDOM PARA CUANDO QUIERAS EJECUTAR MULTIPLES INTSTANCIAS DEL SERVICIO/MICROSERVICIO
eureka:
  instance:
      prefer-ip-address: true
#PARA DECLARAR IDs ALEATORIOS
#    instance-id:
#    instance-id: ${spring.application.name}:${spring.application.instance_id:${random.value}}
  client:
    fetch-registry: true
    register-with-eureka: true
    serviceUrl:
      defaultZone: http://localhost:8761/eureka
```
