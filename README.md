🎧 Arquivos de Configuração para ESP32-A1S (Audio Kit v2.2)
Este repositório contém arquivos adaptados para garantir o funcionamento correto da placa ESP32-A1S Audio Kit v2.2 (AI Thinker) com o ESP-ADF (ESP Audio Development Framework).

✅ Objetivo
Permitir que o framework ESP-ADF reconheça corretamente os GPIOs, drivers de áudio e a pinagem da sua placa AI Thinker v2.2, substituindo os arquivos da LyraT v4.3.

📦 Arquivos Disponíveis
Os seguintes arquivos estão incluídos neste repositório:

board.c

board.h

board_def.h

board_pins_config.c

⚙️ Como Usar no Projeto ESP-ADF
Clone este repositório (ou baixe como ZIP):

bash
Copiar
Editar
git clone https://github.com/viniciusmbs/audio_board.git
Copie os arquivos para substituir os da LyraT v4.3:

bash
Copiar
Editar
cp audio_board/*.c ~/esp/esp-adf/components/audio_board/lyrat_v4_3/
cp audio_board/*.h ~/esp/esp-adf/components/audio_board/lyrat_v4_3/
💡 Isso garante que o ESP-ADF use os pinos e codecs corretos da sua placa ESP32-A1S.

🛠️ Para Desenvolvedores
Os arquivos originais do LyraT ainda podem ser recuperados no repositório do ESP-ADF se necessário. Este repositório é voltado exclusivamente para o funcionamento com o Audio Kit v2.2.

🤝 Contribuições
Achou algum erro ou quer melhorar algo? Fique à vontade para abrir uma issue ou enviar um pull request!

📄 Licença
MIT License (ou substitua conforme aplicável)
