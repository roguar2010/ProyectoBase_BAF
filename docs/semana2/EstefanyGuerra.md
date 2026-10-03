# Historias de usuario individuales

**Nombre:** Estefany Carolina Guerra Guerra

**Usuario de GitHub:** Eguerrag

**Producto:** VerifyW3, verificación de certificados y títulos con blockchain

---

## Mis historias de usuario

**HU-01 · Verificador: comprobar autenticidad y estado.** Como **analista de talento humano,** quiero **verificar si la credencial presentada por un candidato es autentica, fue emitida por una institución legítima y sigue vigente,** para **decidir la vinculación sin esperar días ni pedir confirmación manual.**

**HU-02 · Institución: emitir una credencial firmada.** Como **institución emisora,** quiero **registrar en la red la huella criptográfica de cada credencial que expido, firmada con mi propia llave,** para **garantizar que nadie pueda alterarla ni reescribirla.**

**HU-03 · Institución: revocar o reemplazar una credencial.** Como **institución emisora,** quiero **actualizar el estad de una credencial cuando se revoca o sustituye, indicando el motivo y la fecha,** para **que cualquier verificador conozca su situación en tiempo real.**

**HU-04 · Verificador: confirmar que el emisor es legítimo.** Como **analista de talento humano,** quiero **verificar que la institución emisora aparece en un registro autorizado,** para **no aceptar una credencial emitida por una entidad falsa.**

**HU-05 · Titular: compartir sin entregar mis datos personales.** Como **titular de una credencial,** quiero **generar un enlace o QR con solo la credencial que elijo,** para **compartirla sin entregar mi cédula ni autorizar la divulgación de mi información personal.**

**HU-06 · Titular: conservar una prueba que sobreviva al emisor.** Como **titular,** quiero **guardar mi credencial junto con su prueba de registro,** para **poder demostrar mi formación aunque la institución cierre, pierda sus archivos o tenga su portal caído.**

**HU-07 · Titular: centralizar mis credenciales.** Como **titular con varios titulos y certificaciones de varias instituciones,** quiero **ver toda mis credenciales en un único panel y compartir varias con un solo enlace,** para **predentarlas juntas en un solo proceso de selección.**

## La más importante y por qué

> Organiza las historias de mayor a menor importancia: en la primera fila va la más importante. En cada fila indica el número de la historia y por qué la ubicaste en esa posición. Si usaste menos de 7 historias, borra las filas que sobren.

| Orden de importancia | Historia # | Por qué |
| :---: | :---: | --- |
| 1 | **HU-01** · Verificador: comprobar autenticidad y estado. | Es la hipótesis central del Problem Brief y la métrica del MVP: pasar de días a menos de un minuto y detectar el 100 % de los documentos alterados o revocados. Resuelve F1, F2 y F4 a la vez: el documento recibido no prueba nada por sí mismo, la verificación tarda días y las revocaciones no se propagan. Si no funciona, el producto no tiene razón de ser. |
| 2 | **HU-02** · Institución: emitir una credencial firmada. | Es la condición previa de todo lo demás: sin credenciales registradas no hay nada que verificar. Cumple el primer criterio de pertinencia del Problem Brief, porque varias partes que no confían entre sí comparten el mismo registro. Va segunda porque por sí sola no entrega valor hasta que alguien verifica. |
| 3 | **HU-03** · Institución: revocar o reemplazar una credencial. | Resuelve F4 directamente: la verificación actual es una fotografía de un momento, no un estado consultable en el tiempo. Con HU-01 y HU-02 cierra el ciclo mínimo: emitir, verificar, revocar y verificar de nuevo. Demuestra la inmutabilidad, porque cada cambio queda como un nuevo evento sin reemplazar el anterior. |
| 4 | **HU-04** · Verificador: confirmar que el emisor es legítimo. | Cubre el Supuesto 2 del proyecto: la cadena prueba que el registro no cambió, pero no que quien lo escribió sea legítimo. Sin ella, el “certificado falso” se convierte en el “emisor falso”. En el MVP puede resolverse con una lista curada de instituciones autorizadas. |
| 5 | **HU-05** · Titular: compartir sin entregar mis datos personales. | Mejora mucho la experiencia del usuario principal y responde a F5 y al Supuesto 3 (Ley 1581). No es indispensable para demostrar el MVP, porque el verificador ya puede comprobar directamente el archivo que recibe. |
| 6 | **HU-06** · Titular: conservar una prueba que sobreviva al emisor. | Resuelve F6 y aprovecha una ventaja propia del registro distribuido. Pesa menos al inicio, porque con emisores nuevos y activos el cierre de una institución es poco frecuente. |
| 7 | **HU-07** · Titular: centralizar mis credenciales. | Ataca F3 desde el lado del titular, pero solo aporta valor cuando hay varios emisores en la red. Es la más prescindible para un primer MVP. |

**La más importante es HU-01.** Ya que representa la prueba de valor del producto. Un tercero que no conoce al candidato ni a la institución debe poder comprobar, en segundos y sin intermediarios, que una credencial es auténtica, no fue alterada y sigue vigente. Es el criterio central del Problem Brief y la métrica del MVP, porque si esta verificación no ocurre en minutos y con confianza, la solución no tiene razón de ser. La experiencia de consultar y validar una credencial es la que debe funcionar en la demostración del producto y la que valida la hipótesis de valor.