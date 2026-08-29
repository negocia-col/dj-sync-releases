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

La primera vez macOS dirá que es de un desarrollador no identificado.
**Clic derecho sobre la app → Abrir** (no doble clic). Solo hace falta una vez.
