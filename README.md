# DJ Sync

**Una herramienta de escritorio para DJs: mantiene tu biblioteca ordenada y te
dice la calidad real de cada archivo.**

Un MP3 puede decir 320 kbps y no serlo. Si alguien tomó uno de 128 y lo volvió a
exportar, pesa igual pero le falta el brillo de arriba: en audífonos no se nota,
en un equipo grande sí. DJ Sync mira el audio por dentro —no lo que el archivo
dice de sí mismo— y te señala cuáles hay que reemplazar. En una biblioteca real
de 284 canciones encontró 55 que no eran lo que decían.

Qué hace:

- **Verifica la calidad de verdad.** Analiza el espectro de cada archivo y
  distingue un 320 auténtico de uno inflado, con la prueba visual a la vista.
- **Ordena por lista.** Pega el enlace de una playlist y arma su carpeta, con el
  formato al inicio de cada nombre (`FLAC …`, `MP3 320 …`).
- **Te ayuda a comprarla.** Cuando una canción no aparece o la que hay es mala,
  te lleva a comprarla en Beatport, Bandcamp o Traxsource — que es lo único que
  le llega al artista.

Hecha por un DJ, para su propio set. Mac y Windows.

---

## Sobre este repositorio

Aquí se publica **cuál es la última versión de DJ Sync y dónde bajarla**. Nada más:
el código de la aplicación no vive en este repositorio.

- `latest.json` — la versión actual y el enlace de descarga de cada sistema.
- **Releases** (a la derecha) — los instaladores para Mac (`.dmg`) y Windows (`.exe`).

La app consulta este archivo al abrirse y avisa cuando hay algo nuevo. Instalar es
descargar y reemplazar: la configuración, la licencia y tu música no se tocan,
porque viven en una carpeta aparte de tu usuario.

## Instalar en Mac

Abre el `.dmg` y arrastra DJ Sync a la carpeta Aplicaciones.

La primera vez, macOS dirá que la app es de un desarrollador no identificado.
Es normal: DJ Sync no está firmada por Apple. Cómo autorizarla depende de tu
versión de macOS.

**macOS 15 (Sequoia) o más nuevo**

1. Intenta abrirla con doble clic. Saldrá el aviso; ciérralo.
2. Ve a **Ajustes del Sistema → Privacidad y Seguridad**.
3. Baja hasta abajo: aparece que DJ Sync fue bloqueada, con el botón
   **«Abrir de todos modos»**. Dale ahí.

**macOS 14 (Sonoma) o anterior**

**Clic derecho sobre la app → Abrir**, y **Abrir** otra vez en el aviso.

> El atajo del clic derecho **dejó de funcionar en Sequoia** — Apple lo quitó.
> Si lo intentas ahí y no pasa nada, no es que la app esté rota: es que ese
> camino ya no existe y hay que ir por Ajustes del Sistema.

En los dos casos solo hace falta una vez. A partir de ahí abre con doble clic
como cualquier otra app.

### Si dice que la app «está dañada»

No lo está. Es la marca de cuarentena que macOS le pone a lo que se baja de
internet. Se quita pegando esto en la Terminal, y luego se abre normal:

```
xattr -cr "/Applications/DJ Sync.app"
```

Ese aviso **solo sale si el archivo llegó con cuarentena** — bajado de internet
o por AirDrop. Copiado desde una memoria USB llega limpio y abre sin pelear.

### Mac con chip M1, M2 o M3

Si al abrirla te ofrece instalar Rosetta, acepta. Es de Apple y se instala solo.
