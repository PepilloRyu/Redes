
# LAB 2 – Cable Crossover

## Objetivo
Aprender a conectar dispositivos del mismo tipo usando un cable Crossover  
(p. ej., PC ↔ PC o Switch ↔ Switch cuando no hay puertos uplink automáticos).

## Topología
![alt text](Imagenes/00_01_02_01.png)

## Pasos

1. Arrastra dos PC al área de trabajo.  

   ![alt text](Imagenes/00_01_02_02.png)

3. Selecciona el cable **Copper Crossover**.

   ![alt text](Imagenes/00_01_02_03.png)

5. Conecta:
   - PC0 FastEthernet0 → PC1 FastEthernet0  

   ![alt text](Imagenes/00_01_02_04.png)
   

6. Configuración de la PC0
- IP: 192.168.2.10  
- Máscara: 255.255.255.0

     ![alt text](Imagenes/00_01_02_05.png)

5. Configuración de la PC1
- IP: 192.168.2.20  
- Máscara: 255.255.255.0

     ![alt text](Imagenes/00_01_02_06.png)

6. Verifica conectividad:

Desde PC0:
```bash
ping 192.168.2.20
```

![alt text](Imagenes/00_01_02_07.png)

Desde PC1:
```bash
ping 192.168.2.10
```

![alt text](Imagenes/00_01_02_08.png)

## Resultado
Ambas PCs deben poder hacerse ping entre sí usando un cable crossover.

![alt text](Imagenes/00_01_02_09.png)


