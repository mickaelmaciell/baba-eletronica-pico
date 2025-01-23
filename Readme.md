# Babá Eletrônica com Raspberry Pi Pico W (BitDogLab)

## Descrição
Este projeto implementa uma **Babá Eletrônica** utilizando a **Raspberry Pi Pico W**. Ele monitora sons no ambiente e executa ações específicas como:
- **Tocar uma melodia** quando sons são detectados.
- **Exibir informações** no display OLED sobre o status do sistema.
- Utilizar um **indicador visual com LEDs RGB** para mostrar o estado do sistema:
  - Azul: Sistema aguardando.
  - Verde: Sistema ativo.
  - Vermelho: Som detectado.
- Ativação e desativação do sistema por botões físicos.

O projeto é ideal para demonstrações de sistemas embarcados e pode ser adaptado para outros cenários de monitoramento de som.

## Funcionalidades
- **Detecção de Som**: O sistema utiliza um microfone para detectar sons no ambiente.
- **Melodia**: Reproduz "Brilha, Brilha Estrelinha" no buzzer ao detectar som.
- **Controle de Estado**:
  - Botão A: Ativa o sistema.
  - Botão B: Desativa o sistema.
- **Display OLED**: Exibe mensagens sobre o status do sistema.
- **LED RGB**: Indica o estado atual do sistema:
  - Azul: Sistema aguardando ativação.
  - Verde: Sistema ativo.
  - Vermelho: Som detectado.

## Requisitos de Hardware
- **Raspberry Pi Pico W**
- **Display OLED SSD1306**
- **Buzzer Passivo**
- **Microfone Analógico**
- **Botões (2 unidades)**
- **LED RGB**
- **Protoboard e Jumpers**

## Requisitos de Software
- **Raspberry Pi Pico SDK**
- **Biblioteca SSD1306**
- **Ferramentas de Desenvolvimento**:
  - Visual Studio Code com extensões para C/C++ e Pico SDK
  - CMake para geração de builds

## Como Usar
1. **Configuração de Hardware**:
   - Conecte os componentes como descrito na seção de hardware.
2. **Configuração de Software**:
   - Clone o repositório: 
     ```bash
     git clone https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
     ```
   - Compile o código utilizando o CMake:
     ```bash
     cd pasta_do_projeto
     mkdir build && cd build
     cmake ..
     make
     ```
3. **Upload para a Raspberry Pi Pico**:
   - Conecte sua Pico W via USB e arraste o arquivo `.uf2` gerado para a unidade.

## Estrutura do Projeto
- baba_eletro_embarca/
- ├── CMakeLists.txt        # Configuração do CMake
- ├── display_oled.c        # Código principal
- ├── inc/
- │   ├── ssd1306.h         # Header do display OLED
- ├── src/
- │   ├── ssd1306.c         # Driver do display OLED
- └── README.md             # Documentação do projeto
## Demonstração
- [Link para o vídeo no YouTube](https://www.youtube.com/watch?v=NBzkNKW0teI)

Licença
Este projeto está sob a licença MIT.

Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.







