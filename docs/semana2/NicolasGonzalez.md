# Historias de usuario individuales

**Nombre:** Nicolás González Franco

**Usuario de GitHub:** [@FRANGONICOLAS](https://github.com/FRANGONICOLAS)

**Producto:** VerifyW3, verificación de certificados y títulos con blockchain

---

## Mis historias de usuario

**HU-01 · Reclutador: comprobar un certificado**:
Como **reclutador de una empresa**, quiero **comprobar que el certificado que me envió un candidato es auténtico**, para **decidir su contratación sin esperar días a que la institución me responda**.

**HU-02 · Institución: registrar un certificado**:
Como **institución educativa**, quiero **registrar en VerifyW3 cada certificado que entrego**, para **que las empresas lo comprueben sin tener que escribirme**.

**HU-03 · Reclutador: consultar si sigue vigente**:
Como **reclutador de una empresa**, quiero **saber si un certificado sigue vigente**, para **no contratar a alguien con un certificado anulado**.

**HU-04 · Institución: anular un certificado**:
Como **institución educativa**, quiero **anular un certificado que entregué por error**, para **que las empresas que lo consulten sepan que ya no es válido**.

**HU-05 · Reclutador: ver quién lo entregó**:
Como **reclutador de una empresa**, quiero **ver el nombre de la institución que entregó el certificado**, para **confiar en que viene de una institución reconocida y no de una falsa**.

**HU-06 · Egresado: compartir un certificado**:
Como **egresado que busca empleo**, quiero **compartir mi certificado con un enlace**, para **no enviar copias de mi cédula a cada empresa**.

**HU-07 · Egresado: reunir mis certificados**:
Como **egresado con certificados de varias instituciones**, quiero **reunir todos mis certificados en un solo lugar**, para **presentarlos juntos cuando busco empleo**.

---

## La más importante y por qué

| Orden | Historia | Por qué ocupa este lugar |
|:---:|---|---|
| 1 | **HU-01** Reclutador: comprobar un certificado | Es la hipótesis central del Problem Brief y la métrica del MVP: pasar de días a menos de un minuto y detectar el 100 % de los certificados alterados. Si esto no funciona, el producto no tiene razón de ser. |
| 2 | **HU-02** Institución: registrar un certificado | Es la condición previa de todo lo demás: sin certificados registrados no hay nada que comprobar. Va segunda porque por sí sola no le entrega valor a nadie hasta que alguien comprueba. |
| 3 | **HU-03** Reclutador: consultar si sigue vigente | Resuelve F4, que el proceso actual no cubre: hoy la verificación es una foto de un momento. Es parte de la oportunidad priorizada. |
| 4 | **HU-04** Institución: anular un certificado | Es la otra cara de HU-03: sin la acción de la institución no hay estado que consultar. Además demuestra la inmutabilidad, porque la anulación se agrega como un evento nuevo y no borra el registro anterior. |
| 5 | **HU-05** Reclutador: ver quién lo entregó | Cubre el riesgo más grande del Problem Brief (Supuesto 2): la cadena prueba que el registro no cambió, pero no quién lo escribió. Queda debajo de las cuatro primeras porque en el MVP puede resolverse con una lista curada de instituciones. |
| 6 | **HU-06** Egresado: compartir un certificado | Mejora mucho la experiencia del usuario principal y reduce la circulación de datos personales, pero en el MVP el reclutador puede comprobar el archivo que recibe directamente (HU-01). |
| 7 | **HU-07** Egresado: reunir mis certificados | Aporta valor a largo plazo, pero solo tiene sentido cuando haya varias instituciones en la red. Es la más prescindible para un primer MVP. |

**La más importante es HU-01.** Todo el producto existe para que un tercero que no confía en el candidato ni conoce a la institución pueda comprobar por sí mismo, sin intermediarios, que un certificado es auténtico. Ese es el criterio 3 de pertinencia del Problem Brief (eliminar al intermediario que solo conecta la confianza) y es la experiencia que debe funcionar en la demostración del MVP. Las historias 2 a 4 forman con ella el ciclo mínimo del producto: **registrar → comprobar → anular → comprobar de nuevo**.
