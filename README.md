# Boomer Tractor Simulation

Este repositório contém um controlador em **C** para simulação do trator **New Holland Boomer 3040/3045/3050** no [Webots](https://cyberbotics.com/).

O arquivo principal é [`main.c`](main.c), que implementa o controle do veículo, leitura de sensores e interação via teclado.

---

## 🚜 Funcionalidades

- Controle do trator em ambiente 3D no Webots.  
- Uso do teclado para:
  - **↑** / **↓**: acelerar ou reduzir a velocidade.  
  - **←** / **→**: esterçar à esquerda/direita.  
  - **Barra de espaço**: parar o trator.  
- Sensores habilitados:
  - **Câmera** (com resolução, FOV e captura de imagens).  
  - **GPS** (posição e cálculo de velocidade real).  
  - **LIDAR SICK LMS 291** (com alcance, FOV e resolução).  
- Atuadores:
  - **Motores das rodas dianteiras e traseiras**.  
  - **Motores de esterçamento** (direção).  
  - **Faróis, lanternas traseiras e setas piscando** (controle automático de LEDs).  

---

## 📦 Estrutura do Projeto

```

boomer/
├── main.c          # Código-fonte principal (controlador do trator)
└── README.md       # Documentação

````

---

## ⚙️ Requisitos

- [Webots R2023b](https://cyberbotics.com/) ou superior.  
- Compilador C (GCC ou equivalente).  

---

## ▶️ Como executar

1. Clone este repositório:

   ```bash
   git clone https://github.com/vitor-souza-ime/boomer.git
   cd boomer
````

2. Abra o **Webots** e carregue o mundo que contenha o trator **Boomer**.
   (Certifique-se de que o controlador esteja configurado para usar `main.c`).

3. Compile e rode a simulação:

   * Pressione **Run** no Webots.
   * Use as teclas descritas acima para controlar o trator.

---

## 📝 Licença

Este projeto é distribuído sob a licença [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0).
Consulte o cabeçalho do arquivo [`main.c`](main.c) para mais detalhes.

---

## 📚 Referências

* [Documentação do Webots](https://cyberbotics.com/doc/guide/index)
* [Tractorbook – New Holland Boomer 3040/3045/3050](https://www.tractorbook.de/traktoren/new-holland/boomer-3040-3045-3050/technische-daten/)
