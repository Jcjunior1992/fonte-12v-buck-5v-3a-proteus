# Buck 12V para 5V 3A - LM2596 | Fonte 12V Legacy

> Evolução da fonte linear LM317K + TIP41 11.9V (8R 20W) para Buck switching 5V 3A com LM2596, sem TIP41.


---

### Esquemático

<img width="1132" height="433" alt="image" src="https://github.com/user-attachments/assets/67559c8c-5ff1-45e6-8242-e38372b6d8dc" />

### 3D Image

<img width="848" height="636" alt="image" src="https://github.com/user-attachments/assets/42201380-4de2-422b-974a-4816004bf9b2" />

### PCB Layout

<img width="521" height="602" alt="image" src="https://github.com/user-attachments/assets/7bd5878d-be3c-4a75-b052-7cf75ebffb61" />


### 🔄 Histórico

**v1.0 - Fonte Original 11.9V (funcionando)**
- Transformador 12Vac + KBU4A + 22000uF = 23.5V
- LM317K (TO-3) + TIP41 booster
- Saída: 11.9V @ 1.49A com R 8R 20W

**v2.0 - Atual - Buck 5V 3A (SEM TIP41)**
- LM2596S-ADJ (TO-263-5) já tem chave 3A interna
- Não precisa de TIP41
- Eficiência ~85% vs ~50% da linear

### ⚡ Especificações v2.0

| Parâmetro | Valor |
|---|---|
| Vin | 10V a 24V (vem do mesmo C1 22000uF) |
| Vout | 5.0V fixo |
| Iout | até 3A contínuo |
| Indutor | 33uH a 100uH 4A toroidal amarelo |
| Diodo | 1N5822 Schottky 3A 40V  |
| Ripple | < 50mV com 470uF Low ESR |

### 📦 BOM  

- 1x LM2596S-5.0 ou LM2596S-ADJ
- 1x Indutor toroidal 33uH/100uH 4A - R$ 12
- 1x 1N5822
- 1x 470uF 16V Low ESR (saída)
- 1x 470uF 35V (entrada)
- 2x 100nF cerâmico
- Se usar ADJ: R1 3k0 1% + R2 1k 1% = 4.92V

Fórmula ADJ: `Vout = 1.23 * (1 + R1/R2)`

