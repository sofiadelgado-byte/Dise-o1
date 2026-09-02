flowchart BT

A1["Traumatismo de alta energía asociado al tránsito<br>(1, 6, 10, 12, 15)"]
A2["Fractura expuesta de miembro inferior<br>(2, 7, 9)"]
A3["Lesión de tejidos blandos y estructuras óseas<br>(2, 7)"]
A4["Proceso de recuperación y rehabilitación prolongado<br>(2, 15, 16)"]

B1["Acortamiento del miembro afectado<br>(2, 3, 8, 9)"]
B2["Discrepancia de longitud entre miembros inferiores<br>(3, 4, 5, 17)"]
B3["Distribución asimétrica de cargas y compensaciones biomecánicas<br>(3, 14, 17)"]
B4["Sobrecarga y fatiga muscular<br>(3, 13, 17)"]

C1["Diagnóstico de osteopenia<br>(18)"]
C2["Menor resistencia ósea y necesidad de controlar las cargas durante la recuperación<br>(18)"]

P["PROBLEMA CENTRAL<br><br>Limitación de la movilidad y autonomía en las actividades cotidianas posterior a un accidente de tránsito con fractura expuesta de miembro inferior y diagnóstico de osteopenia"]

E1["Alteración de la marcha<br>(3, 14, 17)"]
E2["Dolor, fatiga y sobrecarga del miembro inferior<br>(3, 14, 17)"]
E3["Dificultad para realizar actividades cotidianas<br>(3, 15)"]

H1["Reducción de la autonomía personal<br>(15, 16)"]
H2["Mayor dependencia de terceros para algunas tareas<br>(15, 16)"]
H3["Restricción de la participación social y laboral<br>(12, 15)"]
H4["Dificultad para retomar actividades habituales<br>(3, 15)"]
H5["Disminución de la calidad de vida<br>(3, 15)"]

A1 --> A2
A2 --> A3
A3 --> P
A4 --> P

A2 --> B1
B1 --> B2
B2 --> B3
B3 --> B4
B4 --> P

C1 --> C2
C2 --> P

B2 --> P

P --> E1
P --> E2
P --> E3

E1 --> H3
E1 --> H4

E2 --> H1
E2 --> H2

E3 --> H1
E3 --> H2
E3 --> H4
E3 --> H5

classDef causa fill:#E8F5E9,stroke:#388E3C,stroke-width:2px,color:#1B1B1B;
classDef subcausa fill:#F1F8E9,stroke:#689F38,stroke-width:2px,color:#1B1B1B;
classDef problema fill:#FFF3E0,stroke:#E65100,stroke-width:4px,color:#1B1B1B;
classDef efecto fill:#E3F2FD,stroke:#1976D2,stroke-width:2px,color:#1B1B1B;
classDef consecuencia fill:#F3E5F5,stroke:#7B1FA2,stroke-width:2px,color:#1B1B1B;

class A1,A2,A3,A4,C1 causa;
class B1,B2,B3,B4,C2 subcausa;
class P problema;
class E1,E2,E3 efecto;
class H1,H2,H3,H4,H5 consecuencia;
