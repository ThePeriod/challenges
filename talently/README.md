# Talently
### **Expectativas de la prueba**

Según la data que te brindamos:

- ¿Qué perfiles son los que tienen más probabilidad de ser:
    - Aceptados en el programa
    - Pagar la matrícula de inscripción
    - Encontrar trabajo en corto tiempo
- ¿Qué otra  información valiosa en base a estas fuentes de datos puedes extraer?

*Los resultados de tus hallazgos aterrizarlos en una PPT con la visualización de datos

### Solución
1. Probabilidad de que un Perfil sea Aceptados en el programa = 
Cantidad de Aceptados de un perfil / 
Cantidad de Postulantes de un perfil

1.1 Cantidad de Aceptados de un perfil =
Cuenta de IDs con tag='postulante-aceptado' y perfil=PERFIL
1.2 Cantidad de Postulantes de un perfil =
Cuenta de IDs con perfil=PERFIL

2. Probabilidad de pagar la matricula de inscripcion =
Cantidad de Aceptados de un perfil que pagan la matricula
Cantidad de Aceptados de un perfil

2.1 Cantidad de Aceptados de un perfil que pagan la matricula =
Cuenta de IDs con tag='postulante-aceptado' y tag='pago-realizado' o 'paid-contact' y perfil=PERFIL

3. Probabilidad de Encontrar Trabajo en Corto Tiempo =
Define: Corto Tiempo (CT)
Menor a la Mediana de todos los tiempos en que un egresado consigue trabajo
Define: Tiempo en que un egresado consigue trabajo
Diferencia de fechas entre kick-off y Placement Date
Mediana = 81

Cantidad de Egresados de un perfil que encuentran trabajo en Corto Tiempo /
Cantidad de Egresados de un perfil que encuentran trabajo

Cuenta de IDs con profile=PERFIL y Placement Date - Kick-Off < 81 y Placement Date <> nan /
Cuenta de IDs con profile=PERFIL y Placement Date <> nan
