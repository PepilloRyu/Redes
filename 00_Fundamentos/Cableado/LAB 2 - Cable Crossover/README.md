# LAB 2 – Cable Crossover

## Objetivo
Aprender a conectar dispositivos del mismo tipo usando un cable Crossover  
(p. ej., PC ↔ PC o Switch ↔ Switch cuando no hay puertos uplink automáticos).

## Topología
![alt text](Imagenes/image-topologia.png)

## Pasos

1. Arrastra dos PC al área de trabajo.  

   ![alt text](Imagenes/image-7.png)

3. Selecciona el cable **Copper Crossover**.
    ![alt text](Imagenes/image-1.png)

4. Conecta:
   - PC0 FastEthernet0 → PC1 FastEthernet0  

   ![alt text](Imagenes/image-2.png)
   

5. Configuración de la PC0
- IP: `192.168.2.10`  
- Máscara: `255.255.255.0`

     ![alt text](Imagenes/image-3.png)

5. Configuración de la PC1
- IP: `192.168.2.20`  
- Máscara: `255.255.255.0`

     ![alt text](Imagenes/image-4.png)

6. Verifica conectividad:

Desde PC0:
```bash
ping 192.168.2.20
```

![alt text](Imagenes/image-5.png)

Desde PC1:
```bash
ping 192.168.2.10
```

![alt text](Imagenes/image-6.png)

## Resultado
Ambas PCs deben poder hacerse ping entre sí usando un cable crossover.

![alt text](Imagenes/image-resultado.png)


