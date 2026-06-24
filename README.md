# VRC / HRV RRi Analyzer Pro v10.5

## Cambios v10.3

- Ajuste a la captura de Kubios Advanced Settings II:
  - SampEn/ApEn: m=2, r=0.2 x SD.
  - DFA alpha1: 4-12 beats.
  - DFA alpha2: 13-64 beats.
  - RQA/D2: embedding dimension=10.
  - RQA threshold=3.1623 x SD.
- Entropías con λ=500 verificable mediante columnas de control:
  - Entropy_lambda
  - Entropy_SD_ms
  - Entropy_r_ms
  - Entropy_N
- MSE: eliminado pseudoconteo A=0.5 introducido en v10.2 porque inflaba escalas altas.
- MSE1 sigue siendo igual a SampEn.


## v10.4
- Añade módulo de diagnóstico Kubios SampEn/MSE en la pestaña No lineales / MSE.
- Para cada escala MSE muestra:
  - N,
  - SD de escala,
  - SD de referencia,
  - r = 0.2 x SD,
  - B matches,
  - A matches,
  - A/B,
  - SampEn calculado,
  - estado: Calculado, A=0, B=0 o puntos insuficientes.
- Permite descargar el diagnóstico en CSV.


## v10.5
- El diagnóstico Kubios SampEn/MSE ahora también aparece dentro del informe automático.
- Para cada fase incluye tabla:
  Fase, Escala, N, r ms, B matches, A matches, A/B, SampEn app y Estado.
