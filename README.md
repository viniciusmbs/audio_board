README para o Projeto audio_board
Este repositório contém os arquivos de configuração específicos para o ESP32-LyraT v4.3 utilizados em projetos que dependem do ESP-ADF (ESP-Audio Development Framework). O objetivo principal é garantir o correto funcionamento dos GPIOs e dos drivers de áudio com a placa LyraT v4.3.

Visão Geral e Propósito
Ao trabalhar com o ESP-ADF, é crucial que os arquivos de configuração da placa de áudio (board.c, board.h, board_def.h, board_pins_conf.c) estejam alinhados com a versão específica do hardware que você está utilizando. Este projeto fornece a versão correta desses arquivos para a placa ESP32-LyraT v4.3.

Instruções de Configuração no Projeto VoIP
Para que seu projeto VoIP (ou qualquer outro projeto ESP-ADF) funcione corretamente com a placa ESP32-LyraT v4.3, siga os passos abaixo para substituir os arquivos de configuração:

Navegue até o diretório do seu projeto ESP-ADF:

Bash

cd ~/esp/esp-adf/components/audio_board
Substitua os arquivos de configuração:
Os arquivos específicos para a LyraT v4.3 já estão incluídos neste repositório, na pasta esp32_audio_kit_v2_3. Você precisará copiar os seguintes arquivos de lá para a pasta lyrat_v4_3 dentro do diretório ~/esp/esp-adf/components/audio_board:

board.c

board.h

board_def.h

board_pins_conf.c

Você pode fazer isso manualmente ou usando os seguintes comandos (assumindo que você está no diretório ~/esp/esp-adf/components/audio_board e que os arquivos já estão na pasta esp32_audio_kit_v2_3 dentro do seu repositório local audio_board):

Bash

cp /caminho/para/o/seu/repositorio/audio_board/esp32_audio_kit_v2_3/board.c ./lyrat_v4_3/
cp /caminho/para/o/seu/repositorio/audio_board/esp32_audio_kit_v2_3/board.h ./lyrat_v4_3/
cp /caminho/para/o/seu/repositorio/audio_board/esp32_audio_kit_v2_3/board_def.h ./lyrat_v4_3/
cp /caminho/para/o/seu/repositorio/audio_board/esp32_audio_kit_v2_3/board_pins_conf.c ./lyrat_v4_3/
Observação: No comando acima, substitua /caminho/para/o/seu/repositorio/audio_board/ pelo caminho real onde você clonou ou tem a pasta audio_board deste repositório. Se você já tem esses arquivos dentro da pasta lyrat_v4_3 do seu ESP-ADF, não é necessário copiá-los novamente.

Explicação: Essa substituição é fundamental para que os GPIOs e os drivers de áudio da sua placa ESP32-LyraT v4.3 operem corretamente com a versão do firmware do seu projeto.

Para Desenvolvedores
Se você precisar dos arquivos originais de configuração da ESP32-Audio-Kit V2.3, eles estão disponíveis neste repositório, na pasta esp32_audio_kit_v2_3. Você pode copiá-los e substituí-los em seu ambiente conforme a necessidade para outras placas.

Como Contribuir
Se você encontrar melhorias ou tiver atualizações para esses arquivos de configuração, sinta-se à vontade para abrir uma issue ou enviar um pull request.

Licença
[Inserir informações de licença, se aplicável. Por exemplo: MIT License]
