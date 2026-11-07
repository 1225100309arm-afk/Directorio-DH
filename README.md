# Directorio Dolorense 

App en Flutter, hecha con **TDD**, que consume una **API REST local hecha en Node**. Es un directorio de negocios de Dolores Hidalgo: la API guarda la lista y la app la **consulta, agrega, marca favoritos y elimina**. Todo funciona en la red Wi-Fi, sin pagar servidores.



### API en Node

**C1 · `responder()`: siempre JSON + cabeceras CORS**
![C1](capturas/C1_responder.png)

**C2 · Las rutas REST: GET, POST, PUT y DELETE con sus códigos**
![C2](capturas/C2_rutas_rest.png)

**C3 · Escuchar en `0.0.0.0` para que entre el celular**
![C3](capturas/C3_listen.png)

### App Flutter

**C4 · `pubspec.yaml`: se agrega el paquete http**
![C4](capturas/C4_pubspec.png)

**C5 · Traductor JSON ↔ objeto `Negocio`**
![C5](capturas/C5_negocio_json.png)

**C6 · Excepciones con nombre propio y mensaje claro**
![C6](capturas/C6_excepciones.png)

**C7 · `_ejecutar()`: timeout, errores de red y statusCode en un solo lugar**
![C7](capturas/C7_ejecutar.png)

**C8 · `listar()`: GET /negocios y JSON → lista de objetos**
![C8](capturas/C8_listar.png)

**C9 · URL según la plataforma (10.0.2.2, localhost o la IP de la PC)**
![C9](capturas/C9_config_url.png)


**C11 · Los 5 estados de la pantalla**
![C11](capturas/C11_estados.png)

**C12 · `cargar()`: cargando → listo / vacío / error**
![C12](capturas/C12_cargar.png)

**C13 · La pantalla dibuja cada uno de los 5 estados con `switch`**
![C13](capturas/C13_switch_pantalla.png)



**P1 · MockClient revisa el método, la ruta y la respuesta**
![P1](capturas/P1_test_listar.png)

**P2 · Un servidor lento se trata como "sin conexión"**
![P2](capturas/P2_test_timeout.png)


---

