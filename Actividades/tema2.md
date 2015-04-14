#**Ejercicios Tema2**</br></br>
##**Ejercicio 2.1.Calcular la disponibilidad del sistema si tenemos dos réplicas de cada elemento (en total 3 elementos en cada subsistema).**

</br>
Datos sin redundancia de hardware</br>

**A<sub>T</sub> = 85% x 90% x 99.9% x 98% x 85% x 99% x 99.99% x 95% = 59.87%**

</br>
2 elementos de cada componente
</br>
 **A<sub>T</sub>=97.75% x 99% x 99.9999% x 99.96% x 97.75% x 99.99% x 99.99% x 99.75% = 94.3%**
 
Mediante la formula obtendremos la redundancia con 3 elementos:</br>

**A<sub>s</sub> = Ac<sub>n-1</sub> + ( (1 – Ac<sub>n-1</sub> ) x Ac<sub>n</sub> )**
</br>

A<sub>web</sub> = 97,75% + ((1-97,75%) x 85%) = 99,6625%
</br>
A<sub>App</sub> = 99% + ((1-99%) x 90%) = 99,9%
</br>
A<sub>DB</sub> = 99,9999% + ((1-99,9999%) x 99,9%) = 99,9999999%
</br>
A<sub>DNS</sub> = 99,96% + ((1-99,96%) x 98%) = 99,9992%
</br>
A<sub>FW</sub> = 97,75% + ((1-97,75%) x 85%) = 99,6625%
</br>
A<sub>Switch</sub>= 99,99% + ((1-99,99%) x 99%) = 99,9999%
</br>
A<sub>ISP</sub>= 99,75% + ((1-99,75%) x 95%) = 99,9875
</br>
</br>
**A<sub>Total </sub>= 99,6625% x 99,9% x 99,9999999% x 99,9992% x 99,6625% x99,9999% x 99.99% x 99,9875 = 99,30289809%**
</br>

Mejora un 39,4328981%
</br>
##**Ejercicio 2.2.Buscar frameworks y librerías para diferentes lenguajes que permitan hacer aplicaciones altamente disponibles con relativa facilidad.**

**PM2 gestor de procesos de producción para aplicaciones Node.js con un balanceador de carga incorporado.**

**Forever es un gestor**







