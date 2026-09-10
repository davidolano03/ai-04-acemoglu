# AI, Human Cognition and Knowledge Collapse

**David Olano**
Repositorio: <https://github.com/davidolano03/ai-04-acemoglu>

## Resultados de los autores

### Pregunta y problema económico

Acemoglu, Kong y Ozdaglar preguntan cómo una IA agéntica más precisa modifica el esfuerzo humano y, mediante este, el conocimiento general heredado por cohortes futuras. La precisión pública es \(X\) y la precisión específica del agente es

\[
Y=\sigma^{-2}+\lambda_I e+\tau_A,
\]

donde \(e\geq0\) es esfuerzo humano y \(\tau_A\geq0\) es la precisión de la señal de IA. Bajo Assumption 1, \(\Delta_I=0\) y \(\Delta_X>0\), el problema estático es

\[
\max_{e\geq0}\left\{f(0,0)+G(X)\Delta_G+
G(X)G(Y)\Delta_X-\frac{e^\alpha}{\alpha}\right\},
\]

con \(G(z)=2\Phi(\sqrt z)-1\), \(g(z)=G'(z)\), \(\alpha>1\) y \(\lambda_I>0\). El agente atomístico toma \(X\) como dado y no internaliza su aporte al conocimiento futuro. Fuentes: §§3.1-3.3, ecuaciones (4) y (6), pp. impresas 6-12 (PDF pp. 8-14).

### Observation 1: resultado principal

Los autores obtienen

\[
U_{eX}=\Delta_X\lambda_I g(X)g(Y)>0,
\qquad
U_{e\tau_A}=\Delta_XG(X)\lambda_I g'(Y)<0.
\]

El primer signo hace complementarios el conocimiento general y el esfuerzo: un \(X\) mayor eleva el valor de acertar la tarea específica. El segundo hace sustitutos la IA agéntica y el esfuerzo: una \(\tau_A\) mayor eleva \(Y\), pero reduce la ganancia marginal del aprendizaje humano. Fuente: Observation 1, §3.4, p. impresa 13 (PDF p. 15).

Los signos estrictos requieren \(\Delta_X>0\), \(\lambda_I>0\), \(X,Y>0\) y la forma gaussiana que garantiza \(g>0\) y \(g'<0\). Firmar la mejor respuesta, \(e_X>0\) y \(e_{\tau_A}<0\), requiere además interioridad, diferenciabilidad y concavidad estricta. Si \(X=0\), el óptimo es \(e=0\) y el segundo efecto deja de ser estricto. Fuente: Observation 2 y nota 4, §3.5, p. impresa 14 (PDF p. 16).

### Precisión de la IA y bienestar

El bienestar no es necesariamente creciente en \(\tau_A\). Los autores miden la utilidad esperada de una cohorte representativa en estado estacionario. Una IA más precisa aporta información directamente, pero desplaza esfuerzo y reduce indirectamente \(\bar X_h\).

Bajo los supuestos base -incluidos Assumption 1, señales gaussianas, agentes atomísticos y de vida corta, \(\alpha>1\), \(\lambda_I,\lambda_G>0\) y varianzas positivas- y Assumption 2,

\[
\sigma^{-2}\geq\sqrt{2}-1,
\]

existe \(0\leq\tau_A^*<\infty\): el bienestar del estado alto aumenta antes y disminuye después; si \(\tau_A^*=0\), el tramo creciente es vacío. Si \(\alpha-1>1/4\), para \(X_1>0\) la economía converge al estado alto. Si \(\alpha-1<1/4\), \(0\leq\tau_A^*<\tau_A^c\) y el resultado depende también de \(X_1\); para \(\tau_A>\tau_A^c\), el colapso es global. Los teoremas no cubren \(\alpha-1=1/4\). Sin Assumption 2 no se garantiza un pico único, y el bienestar cero del colapso depende de \(\Delta_I=0\). Fuentes: Propositions 10-11, §4.3, p. impresa 26 (PDF p. 28), y Propositions 3, 5 y 7, §§3.7-3.8, pp. impresas 18-22 (PDF pp. 20-24).

## Comprobaciones propias

A partir de las ecuaciones (4) y (6), reconstruí la condición de primer orden interior:

\[
\Delta_XG(X)\lambda_Ig(Y)=e^{\alpha-1}.
\]

También comprobé que

\[
U_{ee}=\Delta_XG(X)\lambda_I^2g'(Y)
-(\alpha-1)e^{\alpha-2}<0,
\]

por lo que la solución interior es única. La diferenciación implícita reproduce \(e_X>0\) y \(e_{\tau_A}<0\). No encontré discrepancias algebraicas con Observation 1; confirmé, además, que los signos estrictos no se extienden a \(X=0\) y que una señal técnicamente mejor no implica bienestar monótono.

## Versión exacta consultada

El análisis usa el archivo local `Paper Acemoglu.pdf`: Daron Acemoglu, Dingwen Kong y Asuman Ozdaglar, *AI, Human Cognition and Knowledge Collapse*, NBER Working Paper 34910, febrero de 2026, 69 páginas físicas. SHA-256: `10FA85CC57D8C28FE14922D603B93B642F0EB1FB456233CFCDADEA9DE3A19F30`. Se verificó la coincidencia bibliográfica con la ficha NBER, pero no la identidad binaria con la copia actualmente alojada por NBER.
