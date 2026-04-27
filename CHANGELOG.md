# Changelog

## [Sprint 1] - Ejercicio 01
### Added
- Inicializacion del repositorio Git en rama Sprint_1.
- Creacion de la estructura de directorios del proyecto.
- Creacion de README.md con objetivo e introduccion.
- Creacion de CHANGELOG.md.

## [Sprint 1] - Ejercicio 02
### Added
- Descarga del dataset raw en urban_flow/data/raw/.
- Analisis exploratorio: primeras filas, tipos de datos y valores nulos.

## [Sprint 1] - Ejercicio 03
### Added
- Normalizacion de fechas al formato YYYY-MM-DD (invalidas -> 1932-01-01).
- Normalizacion de horas al formato HH:MM 24hs (invalidas -> 00:00).
- Normalizacion de ubicaciones: mayusculas y limpieza de caracteres especiales.
- Normalizacion de patentes: formato estandar (invalidas -> NA).
- Eliminacion de filas con nulos en columnas relevantes.
- Eliminacion de outliers por metodo IQR en velocidad_registrada.
- Calculo de exceso_velocidad_real (diferencia simple).
- Calculo de exceso_velocidad (diferencia con tolerancia del 5%).
- Filtrado de registros sin infraccion real.
- Guardado del dataset limpio en urban_flow/data/interim/speeding_fines.csv.

## [Sprint 1] - Ejercicio 04
### Added
- Clase FineAnalyzer con encapsulamiento del DataFrame limpio.
- Metodo ranking_patentes: top 5 patentes mas multadas.
- Metodo ranking_horarios: top 5 horarios con mas multas.
- Metodo exceso_promedio: exceso medio como % sobre velocidad maxima.
- Metodo exceso_real_promedio: exceso medio en km/h.
- Metodo multas_por_ubicacion: conteo de multas por ubicacion.

## [Sprint 1] - Punto 06
### Added
- Calculo del porcentaje de infracciones con fecha invalida (1932-01-01).
- Calculo del porcentaje de infracciones con hora invalida (00:00).
