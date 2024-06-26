![](media/OpenGD77-logo.png)


# Guia do Usuário do OpenGD77

## Para OpenGD77 / OpenGD77S / OpenDM1801* / OpenDM1801A* / OpenRD5R / MD-9600 (RT-90) / MD-UV380 (RT-3S) / MD-UV390 / DM-1701 / RT-84

Para as últimas informações e discussões, por favor se dirija ao forum de desenvolvimento e comunidade (em Inglês) em <https://opengd77.com>

# O firmware NÃO É COMPATÍVEL com a nova versão 2022 do Baofeng DM-1801, ou o novo DM-1801A #

<!-- TOC titleSize:2 tabSpaces:2 depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 skip:0 title:1 charForUnorderedList:* -->

## Índice
* [Guia do Usuário do OpenGD77 / OpenGD77S / OpenDM1801* / OpenDM1801A* / OpenRD5R / MD-9600 (RT-90) / MD-UV380 (RT-3S) / DM-1701 / RT-84](#for-opengd77--opengd77s--opendm1801--opendm1801a--openrd5r--md-9600-rt-90--md-uv380-rt-3s--md-uv390--dm-1701--rt-84)
  * [Introdução](#introduction)
    * [Links de Download e outros recursos](#download-links-and-other-resources)
  * [Instalação](#installation)
  * [Transferindo dados ao Rádio](#transferring-data-to-radio)
  * [Compatibilidade de Codeplug](#codeplug-compatibility)
  * [Variações entre diferentes rádios suportados](#variations-between-different-supported-radios)
  * [Telas principais (modos VFO e Canal)](#main-screens-vfo-and-channel-modes)
    * [Mudando entre o modo FM e o modo DMR](#changing-between-fm-mode-and-dmr-mode)
    * [Mudando o Timeslot no modo DMR](#changing-timeslot-in-dmr-mode)
    * [Ajuste automático de Grupos de Conversa (TalkGroup)/Chamada Privada (PrivateCall) e Timeslot no modo DMR](#automatic-setting-of-talkgroupprivatecall-and-timeslot-in-dmr-mode)
    * [Mudando a largura de banda no modo FM](#changing-bandwidth-in-fm-mode)
    * [Controlando a potência de transmissão](#controlling-tx-power)
    * [Gráfico de barra indicador de sinal](#signal-strength-bar-graph)
    * [Funcionalidade específica da tela de canal](#channel-screen-specific-functionality)
      * [Mudando canais dentro da zona atual](#changing-channels-within-the-current-zone)
      * [Mudando zonas](#changing-zones)
      * [Mostrando a frequência do canal](#displaying-the-channel-frequency)
      * [Mostrando informação específica do canal em FM](#displaying-fm-specific-channel-information)
      * [Operação no reverso de repetidora](#reverse-repeater-operation)
      * [Menu rápido do canal](#channel-quick-menu)
        * [Copiando um canal para o VFO](#copying-a-channel-to-vfo)
        * [Salvar o VFO no canal atual](#read-the-vfo-into-the-current-channel)
        * [Filtro](#filter)
      * [Menu rápido do VFO](#vfo-quick-menu)
        * [Selecionar VFO A ou B](#vfo-selection-a-or-b)
        * [Trocar as frequências TX e RX](#exchange-the-tx-and-rx-frequencies)
        * [Copiar a frequência RX para a frequência TX](#copy-the-rx-frequency-to-the-tx-frequency)
        * [Copiar a frequência TX para a frequência RX](#copy-tx-frequency-to-the-rx-frequency)
        * [Filtro](#filter)
        * [VFO para um novo Canal](#vfo-to-new-channel)
        * [Varredura de tom para CTCSS ou código DCS em FM](#tone-scan-for-ctcss-or-dcs-tone-in-fm)
    * [Funcionalidade específica do DMR (telas VFO e Canal)](#dmr-specific-functionality-vfo-and-channel-screens)
      * [Seleção de Timeslot](#timeslot-selection)
      * [Exibição de indictivo DMR ID e nome](#dmr-id-callsign-and-name-display)
      * [Exibição de Talker Alias](#talker-alias-display)
      * [Seleção de grupo de conversa da lista de TG](#talkgroup-selection-from-the-tg-list)
      * [Atribuição de Timeslot ao grupo de conversa dos Contatos Digitais](#assignment-of-timeslot-to-digital-contact-talkgroup)
      * [Grupo de Conversa mostrado em vídeo reverso](#talkgroup-displayed-in-inverse-video)
      * [Entrada manual do número do Grupo de Conversa](#manual-talkgroup-number-entry)
      * [Entrada de número de Chamada Privada](#private-call-number-entry)
      * [Seleção do Contato Digital](#digital-contact-selection)
      * [Entrada do número DMR ID da estação](#station-dmr-id-number-entry)
    * [Funcionalidade específica de FM (telas VFO e Canal)](#fm-specific-functionality-vfo-and-channel-screens)
      * [FM e FM Faixa Estreita](#fm-and-fm-narrow)
      * [Tom CTCSS ou Código DCS](#ctcss-tone-or-dcs-code)
      * [Silenciador](#squelch)
      * [Tom de 1750Hz para operação em repetidora](#1750hz-tone-for-repeater-operation)
      * [Transmissão de tons DTMF](#dtmf-tone-transmission)
      * [Entrada de sequencia DTMF e transmissão](#dtmf-sequence-entry-and-transmission)
      * [Transmissão de localização FM APRS](#fm-aprs-location-transmission)
    * [Funcionalidade específica do VFO](#vfo-specific-functionality)
      * [Passo de mudança de frequência acima/abaixo](#frequency-change-updown-step)
      * [Entrada numérica de frequência](#numerical-frequency-entry)
      * [Ajustar a frequência TX, independente da frequência RX](#to-adjust-the-tx-frequency-independent-of-the-rx-frequency)
      * [Varredura de espectro](#spectrum-sweep-scan)
      * [Escuta dupla no VFO](#vfo-dual-watch)
  * [Modo Monitor](#monitor-mode)
  * [Transmitindo](#transmitting)
    * [Bipe de alerta de Timeout](#timeout-warning-beep)
    * [TOT](#tot)
  * [Varredura](#scanning)
    * [Varredura de Canal](#channel-scanning)
    * [Varredura de VFO](#vfo-scanning)
  * [Outras telas](#other-screens)
    * [Travar tela](#lock-screen)
    * [Entrada de texto](#text-entry)
  * [As teclas de controle e botões](#the-control-keys-and-buttons)
  * [O sistema de menus](#the-menu-system)
  * [Teclas rápidas](#quickkeys)
  * [Menu Principal](#main-menu)
    * [Zona](#zone)
    * [RSSI](#rssi)
    * [Informações do Rádio](#radio-info)
      * [Tensão e porcentagem da Bateria](#battery-voltage-and-percentage)
      * [Relógio](#time-clock)
      * [Tela de data](#date-screen)
      * [Tela de local](#location-screen)
      * [Temperatura da CPU](#cpu-temperature)
      * [Histórico de tensão da bateria](#battery-voltage-history)
    * [Contatos](#contacts)
      * [Contatos DMR](#dmr-contacts)
      * [Contatos FM DTMF](#fm-dtmf-contacts)
      * [Novo Contato](#new-contact)
    * [Último ouvido](#last-heard)
    * [Informação do Firmware e créditos](#firmware-info-and-credits)
    * [Opções **(contém as 8 telas de opção seguintes)**](#options)
        * [Opções Gerais](#general-options)
          * [Duração de tecla](#key-long)
          * [Repetição de tecla](#key-rpt)
          * [Autobloqueio](#auto-lock)
          * [Hotspot](#hotspot)
          * [Calibrar Temperatura](#temp-cal)
          * [Calibrar Bateria](#batt-cal)
          * [Calibrar Hora](#time-cal)
          * [Nivel Eco](#eco-level)
          * [Suspender](#suspend)
          * [Inicialização Segura](#safe-power-on)
          * [Autodesligar](#auto-power-off)
          * [APO com RF](#apo-with-rf)
          * [Sat (Modo seguir satélite)](#sat-satellite-follow-mode)
          * [GPS](#gps)
        * [Opções do Rádio](#radio-options)
          * [Limites de Banda](#band-limits)
          * [Temporização do filtro](#filter-time)
          * [Retardo durante varredura](#scan-delay)
          * [Tempo de Varredura](#scan-dwell)
          * [Modo de Varredura](#scan-mode)
          * [Varrer ao ligar](#scan-on-boot)
          * [Silenciador VHF](#xxx-squelch)
          * [Silenciador 200](#xxx-squelch)
          * [Silenciador UHF](#xxx-squelch)
          * [Travar PTT](#ptt-latch)
          * [Permitir PC](#allow-pc)
          * [Potência do usuário](#user-power)
          * [CRC do DMR](#dmr-crc)
        * [Opções de Exibição](#display-options)
          * [Brilho](#brightness)
          * [Nite Bright](#nite-bright)
          * [Brilho Mínimo](#min-bright)
          * [Contraste](#contrast)
          * [Modo](#mode)
          * [Timeout](#timeout)
          * [Tela](#screen)
          * [Auto noite](#auto-night)
          * [Ordem](#order)
          * [Contato](#contact)
          * [Bateria (unidades)](#battery-units)
          * [Informação](#info)
          * [Volume](#volume)
          * [LEDs](#leds)
          * [Fuso Horário](#timezone)
          * [Formato de hora](#time-display-format)
          * [Mostra distância](#show-distance)
        * [Opções de Áudio](#sound-options)
          * [Bipe de Timeout beep](#timeout-beep)
          * [Volume do bipe](#beep-volume)
          * [Bipe DMR](#dmr-beep)
          * [Bipe RX](#rx-beep)
          * [Talker](#talker)
          * [Microfone DMR](#dmr-mic)
          * [Microfone FM](#fm-mic)
          * [Limiar do VOX](#vox-threshold)
          * [Cauda do VOX](#vox-tail)
          * [Prompt](#prompt)
          * [DMR Rx AGC](#dmr-rx-agc)
          * [Supressão de Clique](#click-suppr)
        * [Calibração do Rádio](#calibration-screen)
        * [Idioma](#language)
        * [Opções de Tema](#theme-options)
          * [Seletor de Tema](#theme-chooser)
          * [Opções de Tema](#theme-options)
          * [Seletor de Cor](#colour-picker)
          * [Itens do tema](#here-is-the-detailed-list-of-the-theme-items)
        * [Opções APRS](#aprs-options)
          * [Modo](#beaconing-mode)
          * [Local](#beaconing-location)
          * [Intervalo](#beaconing-initial-interval)
          * [Decaimento](#beaconing-decay-algorithm)
          * [Comprimir](#beaconing-compression)
          * [SmartBeaconing&trade;](#smartbeaconing)
            * [Taxa Lenta](#slow-rate)
            * [Taxa Rápida](#fast-rate)
            * [Velocidade baixa](#low-speed)
            * [Velocidade alta](#high-speed)
            * [Ângulo de giro](#turn-angle)
            * [Inclinação do giro](#turn-slope)
            * [Tempo de giro](#turn-time)
    * [Detalhes do Canal](#channel-details)
      * [Nome do canal](#channel-name)
      * [RX](#rx)
      * [TX](#tx)
        * [Deslocamento da frequência da repetidora](#repeater-shifts)
      * [Modo](#mode)
      * [DMR ID](#dmr-id)
      * [Color Code](#color-code)
      * [Timeslot](#timeslot)
      * [Lista de TG](#tg-lst)
      * [Contato](#contact-1)
      * [Rx CSS](#rx-css-ctcss-or-dcs)
      * [Tx CSS](#tx-css-ctcss-or-dcs)
      * [BW](#bw)
      * [Passo](#step)
      * [TOT](#tot)
      * [Só Rx](#rx-only)
      * [Pular Zona](#zone-skip)
      * [Pular tudo](#all-skip)
      * [VOX](#vox)
      * [Potência do canal](#ch-power)
      * [Silenciador](#squelch-channel)
      * [Bipe](#beep-channel)
      * [Eco](#eco-channel)
      * [TA Tx TS1](#ta-tx-tsx)
      * [TA Tx TS2](#ta-tx-tsx)
	  * [APRS](#aprs-channel)
      * [Aceitando e salvando as mudanças no canal](#accepting-and-saving-the-changes-to-the-channel)
    * [Tela de Satélite](#satellite-screen)
      * [Vista Polar](#polar-view)
      * [Tela de predição individual de satélite](#satellite-individual-predictions-screen)
      * [Tela de dados ao vivo do satélite](#satellite-live-data-screen)
      * [Ajustes de silenciador e potência](#squelch-and-power-settings)
      * [Alarma de satélite](#satellite-alarm)
      * [Integração com CPS](#cps-integration)
      * [Notas técncias](#technical-notes)
    * [Tela do GPS](#gps-screen)
  * [Fazendo e recebendo chamadas privadas DMR](#making-and-receiving-dmr-private-calls)
    * [Fazendo uma chamada privada](#to-make-a-private-call)
    * [Recebendo uma chamada privada](#to-receive-a-private-call)
  * [Modo Hotspot](#hotspot-mode)
  * [Reiniciando as configurações](#resetting-the-settings)
  * [Operação no GD-77S](#gd-77s-operation)
    * [Modo Canal/TG no GD77S](#gd77s-channel--tg-mode)
    * [Modo varredura no GD77S](#gd77s-scan-mode)
    * [Modo timeslot no GD77S](#gd77s-timeslot-mode)
    * [Modo Color Code no GD77S](#gd77s-color-code-mode)
    * [Modo filtro DMR NO GD77S](#gd77s-dmr-filter-mode)
    * [Modo Zona no GD77S](#gd77s-zone-mode)
    * [Modo de potência no GD77S](#gd77s-power-mode)
  * [Específicos do MD-9600 e RT-90](#md-9600-and-rt-90-specific)
  * [Software CPS](#cps-software)
    * [Visão Geral](#overview)
      * [Instalação de novo driver](#new-driver-installation)
      * [Menu do OpenGD77](#opengd77-menu)
      * [PRIMEIRO PASSO IMPORTANTE: Backup primeiro](#backup-before-you-do-anything-else)
      * [Lendo e gravando seu Codeplug](#reading-and-writing-your-codeplug)
      * [Gravando DMR IDs -- o banco de dados do usuário](#writing-dmr-ids----the-user-database)
      * [Melodia inicial](#boot-tune)
        * [Melodia inicial em código Morse](#boot-tune-in-morse-code)
      * [Melodias e notas](#melodies-and-notes)
      * [Imagem inicial](#boot-image)
<!-- /TOC -->


<div style="page-break-after: always; break-after: page;"></div>

![](media/OpenGD77-logo.png)

## Introdução

Esse guia do usuário é um trabalho em andamento, assim como o firmware.

As fotos serão atualizadas quando o firmware em uma área particular estabilizar.

A intenção do projeto é criar um firmware não comercial cheio de recursos que substitua o firmware de fábrica por completo.
Esse firmware foi projetado especificamente para uso **Radioamador**, e tem recursos indisponíveis no firmware oficial.

*Notas:*

- **O firmware ainda está em desenvolvimento e há algumas áreas chave de funcionalidade que são suportadas no firmware oficial mas não neste firmware**
- Tx e Rx de mensagens SMS **não são atualmente suportados**, mas podem ser suportados no futuro.
- Listas de varredura  **não são suportados** porque o recurso de varredura de canal ou zona provê quase a mesma funcionalidade.
- Privacidade e Encriptação **nunca serão** suportados, devido a serem ilegais para uso no radioamador, e desenvolvedores em alguns países (*por ex.* Austrália) são obrigados legalmente a colocar acesso via porta dos fundos em sistemas de encriptação mediante solicitação do governo, assim efetivamente tornando ilegal ou impossível desenvolver sistemas que contenham encriptação.


<div style="page-break-after: always; break-after: page;"></div>

### Links de Download e outros recursos

Por razões de licencamento de software, o firmware OpenGD77 precisa incluir partes do firmware original do fabricante, para fornecer suporte para codificação e decodificação da voz AMBE.
Dependendo do tipo do seu rádio, você vai precisar fazer download e extrair um dos dois seguintes aquivos 'doadores', armazená-los em seu computador e anotar sua localização.

**Arquivo Doador para GD-77 | GD-77S | DM-1801 | DM-1801A | RD-5R**

<https://radioddity.s3.amazonaws.com/2021-01-26%20GD-77%20CPS%20%26%20Firmware%20Changelog%20-%20Ham%20Version.zip>

Descompacte o arquivo zip do firmware doador, extraia o arquivo 'GD-77_V4.3.6.sgl' da pasta "Firmware software V4.3.6" e salve no seu computador.

Note, esse arquivo é o mesmo para todos os tipos de rádio acima.

**Arquivo Doador para TYT MD-9600 | Retevis RT-90 | TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84**

<https://www.passion-radio.com/index.php?controller=attachment&id_attachment=760>

Descompacte o arquivo zip do firmware doador, extraia o arquivo 'MD9600-CSV(2571V5)-V26.45.bin' e salve no seu computador.

Note, esse arquivo é o mesmo para todos os tipos de rádio acima.

**Binários do Firmware:**

**GD-77 | GD-77S | DM-1801 | DM-1801A | RD-5R**
<https://www.opengd77.com/downloads/GD77/Firmware/Latest>

**TYT MD-9600 | Retevis RT-90**
<https://www.opengd77.com/downloads/MD9600/Firmware/Latest>

O MD-9600 | RT-90 foi produzido com múltiplos PLLs e chips de IF diferentes durante a linha de produção.
Você precisa instalar a versão que combina com sua versão de hardware.
A versão está escrita na placa de circuito impresso dentro do topo do rádio, mas algumas vezes a TYT mudou o hardware sem mudar a versão na placa.
Para rádios com versão de hardware 4A use o firmware Versão 5.
Para rádios muito antigos com versão de hardware 2 escrito na placa, pode ser necessário carregar o firmware versão 1.

Nenhum dano irá ocorrer se você carregar a versão de firmware errada. Contudo, o rádio não irá receber ou transmitir.
Assim, basicamente se seu rádio não receber ou transmitir, tente uma versão de firmware para um hardware diferente.

**TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84**
<https://www.opengd77.com/downloads/MDUV380_DM1701/Firmware/Latest/>

*Nota*:

- Versões com JA no nome são traduzidas para usuários japoneses e somente suportam idiomas Inglês e Japonês.

- **OpenGD77 CPS**
<https://www.opengd77.com/downloads/PC_CPS_20230910/Latest>


- **Código Fonte mais recente para o firmware lançado integralmente:**
<https://www.opengd77.com/downloads/releases>


- **Forum do OpenGD77:**
<https://www.opengd77.com/>


<div style="page-break-after: always; break-after: page;"></div>

## Instalação

O firmware pode ser instalado nos seguintes rádios

- Radioddity GD-77 (também conhecido como TYT MD-760)
- Radioddity GD-77S
- Baofeng DM-1801 - SOMENTE HARDWARE VERSÃO 1  (também conhecido como Baofeng DM-860)
- Baofeng DM-1801A - SOMENTE HARDWARE VERSÃO 1
- Baofeng RD-5R (também conhecido como Baofeng DM-5R Tier 2)
- TYT MD-9600 | Retevis RT-90
- TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84


O firmware deve ser instalado usando o menu 'Extras/Firmware Loader' no OpenGD77 CPS. O carregador original de firmware do fabricante não pode ser usado para carregar o firmware OpenGD77.

A instalação do firmware é realizada por conta e risco do proprietário, mas o firmware oficial geralmente pode ser recarregado de volta no rádio se o usuário tiver problemas com o firmware, **desde que o operador faça um backup completo do seu rádio usando o OpenGD77 CPS imediatamente após o firmware tiver sido instalado** (veja [*seção backup*](#backup-before-you-do-anything-else))

*Notas:*

- *O firmware não é compatível com a nova versão 2022 do Baofeng DM-1801 ou DM-1801A, que agora usa hardware interno e eletrônica completamente diferentes.*
- O software oficial Radioddity CPS PC não é compatível com o firmware, e o **OpenGD77 CPS** deve ser usado no lugar. Ele pode ser baixado do link mostrado na [seção 1.1](#download-links-and-other-resources) desse guia. Esse CPS tabém deve ser usado para o Baofeng, TYT, Retevis e todos os outros rádios suportados.

### Transferindo dados para o Rádio

O CPS deve ser usado para instalar o firmware e também para ler e gravar o codeplug, gravar os dados de satélite, prompts de voz, e o banco de dados DMR ID.

1. Atualização do Firmware.
  * Ponha o rádio no modo de atualização de firmware usando:
  
    * Segure os dois botões indicados abaixo (**S1**,**Fn**) e ligue o rádio.
	
      * Radioddity GD-77 ou GD-77s ou TYT MD-760 ou MD-730:
        * Segure os **dois botões menores** próximos ao botão PTT.
      * Baofeng DM-1801 ou DM-1801A ou DM-860:
        * segure os **dois botões menores** abaixo do botão PTT.
      * Baofeng RD-5R or DM-5R Tier2:
        * Os botões laranja **S1** (Call) e preto Fn (**Moni** ou **S2**) (qualquer lado do PTT).
      * TYT MD-9600 | Retevis RT-90
        * Segure os botões P1 e botão laranja, enquanto aplica energia 12V ao rádio. Note que atualizar o firmware OpenGD77 para uma nova versão não requer que a energia seja removida e reconectada, apenas ligue o rádio usando o botão power/verde enquanto segura os botões P1 e laranja, e irá entrar no modo de atualização de firmware.
      * TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84
        * Segure os dois botões no topo do lado do rádio (**S1** e PTT) e ligue o rádio.

		
![buttons layout](media/PTT-layout.png)<!-- { width=420 } -->

  * A tela LCD ficará apagada. Nos rádios de mão, o LED será iluminado ou piscará.

  * Para o GD-77 | GD-77S | DM-1801 | DM-1801A e RD-5R nenhum driver é necessário. 
	Para todos os outros rádios é necessáio o driver STM DFUSe. Se o driver não for instalado automaticamente pelo Windows, você poderá precisar usar o Gerenciador de Dispositivos do Windows para achar e instalar o driver correto.
  
  * Selecione o tipo de rádio
  
  ![firmware loader select radio type](media/cps_radio_type_menu.png)
  
  * O Firmware é instalado facilmente pelo menu Extras no [CPS](#cps-software).  
    ![firmware loader menu access](media/Firmware_loader-01.png)<!-- { width=400 } -->

    - Escolha o modelo do seu rádio.  
      ![firmware loader window for MK22](media/Firmware_loader-02.png)<!-- { width=420 } -->  
      ![firmware loader window for STM32](media/Firmware_loader-03.png)<!-- { width=420 } -->

    - Por razões de licenciamento de software, na primeira vez que você usar o carregador de firmware, deve clicar em 'Select official firmware (donor) file' e então selecionar o arquivo doador que você baixou previamente.

      Só é necessário fazer isso na primeira vez. Se você não fizer, só será possível utilizar o rádio no modo FM.

      **Nota!  Não tente instalar o firmware oficial do fabricante no rádio, isso só é necessário para o CPS poder adicionar funcionalidade DMR ao firmware.**

      Assim que você completar esse procedimento corretamente, a barra de título do carregador de firmware irá mostrar [+DMR].

    - O firmware pode opcionalmente suportar um idioma adicional. Selecione isso no menu descendente 'Additional Language' se precisar.
    - Clique 'Select Open firmware file & Update' ou 'Select a File and Update'
    - Selecione um arquivo de firmware .zip baixado previamente. (O arquivo mais recente pode ser encontrado no local de download dados na [seção 1.1](#download-links-and-other-resources))
      O firmware selcionado será corrigido com dados do firmware oficial e então enviado ao rádio junto com o idioma adicional, se selecionado.
    - Quando o download estiver completo, se o rádio não reiniciar automaticamente, desligue e ligue novamente.
	
 **Nota! O formato de codeplug usado em todos os rádios exceto o GD-77 não é suportado pelo firmware. Assim, você precisará instalar um codeplug no formato OpenGD77 usando o CPS antes de poder usar qualquer função do rádio, exceto VFO - que pode ser mudado manualmente**


2. Atualizando o codeplug usando o [OpenGD77 CPS](#cps-software).
  - Esse mecanismo usa comunicação serial enquanto o rádio está normalmente ligado com o LCD ativo.
    * Se você estava atualizando o firmware, desligue e ligue o rádio para se certificar que saiu deste modo.
    * Ele usa porta serial, assim o driver do OpenGD77 deve estar instlado. Isso ocorre como parte da instalação do  software CPS.
    * Detalhes específicos na [seção CPS](#backup-before-you-do-anything-else)


<div style="page-break-after: always; break-after: page;"></div>

## Compatibilidade de Codeplug

O firmware oficial de cada um desses rádios usa formatos de codeplug ligeiramente diferentes.

Para o melhor uso dos recursos do OpenGD77, recomendamos que você grave um novo codeplug para o rádio usando o OpenGD77 CPS.

O OpenGD77 CPS também é capaz de importar um codeplug existente de arquivos .CSV.

O codeplug só pode ser carregado para o firmware usando o [OpenGD77CPS](#cps-software).

Também é recomendado que você estruture seu codeplug para remover canais duplicados que são na mesma frequência, mas usam Grupos de Conversa (TG) diferentes. Veja a seção [*Programando Canais e Grupos de Conversa para uso com o firmware*](#overview) no final deste guia do usuário.

<div style="page-break-after: always; break-after: page;"></div>

## Variações entre diferentes rádios suportados

Nem todos os rádios suportados tem o mesmo número de botões ou mesmo tamanho de tela, assim há algumas diferenças quando for operar rádios diferentes do Radioddity GD-77.

Além disso, nem todos os rádios suportam todas as funcionalidades.

- O Radioddity GD-77 (também conhecido como *TYT MD-760*), tem dois botões abaixo do PTT. O botão **Preto** é tecnicamente conhcido como **SK1**, e o botão **azul** é conhecido como **SK2**. Esse botão tambem é referenciado aqui nesse manual como o botão **Função**. Esse rádio também tem um botão **Laranja** no topo.
- O hardware USB do Baofeng RD-5R | DM-5R não suporta conexão USB enquanto o rádio está transmitindo, assim **não é possível** usar o modo Hotspot nesse rádio.
- O Baofeng RD-5R | DM-5R não tem os botões das setas direita ou esquerda, assim o botão **A/B** é usado para substituir a seta esquerda e o botão **Band** é usado para substituir a seta direita.
- O Baofeng RD-5R | DM-5R não tem o botão **Laranja**, e essa funcionalidade é simulada usando um **pressionamento longo** no botão colorido laranja **MR/VFO**.
- O Baofeng RD-5R | DM-5R tem 2 botões do lado, mas sua posição é diferente do GD-77 e DM-1801. O botão acima do PTT é usado como o botão **Preto** do lado do GD-77, também conhecido como botão **SK1**. O botão abaixo do PTT é usado como o botão **Função**, também conhecido como **SK2**.
- O Radioddity GD-77S não tem um teclado ou tela, assim sua operação é completamente diferente dos outros rádios suportados que tem uma tela (*veja o apêndice [GD-77S operation](#gd-77s-operation)*).
- O Baofeng DM-1801 | DM-860 tem um botão dedicado **MR/VFO**, que é usado para mudar entre o modo canal e VFO, ao invés de pressionar a tecla de menu **Vermelha**.
- O Baofeng DM-1801 | DM-860 tem um botão dedicado **A/B**,que é usado para mudar entre VFO A e B, ao invés de pressionar o menu rápido via botão **Laranja** no topo do rádio.
- O TYT MD-UV380 | Retevis RT-3S não tem botões de seta esquerda e direita, mas tem um controle rotativo no topo do rádio. Nas telas VFO e Canal, os botões **Acima** e **Abaixo** funcionam igual aos botões Esquerda e Direita no GD-77. O controle rotativo opera funções igual aos botões **Acima** e **Abaixo** do GD-77 e pode ser usado para mudar canal ou frequência do VFO.
- O Baofeng DM-1701 | Retevis RT-84 não tem os botões Esquerda e Direita. P1 é usado como Esquerda, P2 é usado como Direita. O botão **Laranja** é localizado acima do PTT.
Nas telas de menu os botões **Acima** e **Abaixo** se movem para cima e para baixo e o controle rotativo é usado para mudar o valor de cada opção, da mesma forma que os botões Esquerda e Direita fazem no GD-77.
- O TYT MD-9600 | Retevis RT-90 é um radio móvel com botões no painel frontal e no microfone. Veja a seção sobre o MD-9600 para informação sobre teclas e mapeamento de botões.


<div style="page-break-after: always; break-after: page;"></div>

## Telas principais (modos VFO e Canal)

O The firmware tem duas telas principais, a tela VFO e a tela Canal. Essas são similares as telas Canal e VFO do firmware oficial, exceto que elas tem funcionalidades adicionais.

Inicialmente após a instalação do firmware, a tela VFO será mostrada.

![Tela VFO](media/vfo-screen.png)

A frequência usada no VFO para ambos Tx e Rx será lida da configuração *VFO A* do codeplug.

Em ambas as telas VFO e Canal, o modo (**DMR** ou **FM**) é mostrado no canto superior esquerdo do display, e a tensão ou porcentagem da bateria é mostrada no canto superior direito.

No modo **DMR**, o *TimeSlot* atual é mostrado à direita do texto **DMR**, *por ex.* **TS2** para o TimeSlot 2, e o código de cor *Color Code*, *ex.* **C1** para o código de cor 1, é mostrado à esquerda da tensão / porcentagem da bateria. Quando o filtro de TimeSlot está desligado, o indicador **TS1** ou **TS2** está em vídeo reverso.

A potência de transmissão atual é mostrada no meio da parte superior da tela (*ex.* 750mW).

Na tela **VFO**, as frequências de TX e RX são mostradas, assim como o Grupo de Conversa (TalkGroup), quando no modo DMR.

A seta à esquerda do **R** (frequência de recepção) indica que as teclas de seta **Acima** e **Abaixo** e as teclas de entrada numérica irão controlar a frequência de recepção (RX).

A tela de canal mostra a mesma informação na linha superior, mas mostra o **Nome do Canal** (nesse exemplo __*Lee Hill*__) assim como a **Zona** (__*Home DMR*__).

No modo DMR o **TalkGroup** (nesse caso __*ColoradoHD*__), também será mostrado.

![displayed information](media/dmr-screen.png)


Em ambas as telas VFO e Canal:

- Pressione a tecla de menu **Vermelho** para mudar entre as telas VFO e Canal (*Nota:* em rádios iguais ao Baofeng DM-1801 e RD-5R, pressione o botão **MR/VFO** para mudar entre o modo Canal e VFO).
- Pressione a tecla de menu **Verde** para entrar no sistema de menus.
- Pressione **Função + Verde** para acesso rápido a tela dos [Detalhes do Canal](#channel-details), que também pode ser acessada via sistema de menus.

*Nota:*

- O VFO atualmente é um tipo especial de canal; assim a tela [Detalhes do Canal](#channel-details) também funciona para o VFO.

### Alternando entre os modos FM e DMR

- Pressione as teclas **SK2** + **Estrela** para alternar entre os modos FM e DMR, em ambas as telas **VFO** ou **Canal**.

### Mudando o Timeslot no modo DMR

- No modo DMR, pressionar a tecla **Estrela** alterna entre *TimeSlot 1* e *TimeSlot 2* e define a opção escolhida como substituição temporária da configuração atual do Timeslot (Timeslot Override).

Para apagar o Timeslot override, pressione e segure a tecla **Estrela** (também conhecida como asterisco).

### Ajuste automático de grupo de conversa (Talkgroup), chamada privada (PrivateCall) e Timeslot no modo DMR

Quando no modo DMR, se o filtro DMR estiver desligado, é possível ajustar automaticamente o rádio para o Talkgroup (TG) correto (mesmo se ele **não** estiver na lista de TG ou definido como contato do canal) durante a recepção:

 - Enquanto estiver recbendo, aprete o botão SK2 uma vez, o rádio irá ativar o Talkgroup override (substituição temporária do grupo de conversa) por conta própria.

*Nota:*

- Se o filtro de Timeslot estiver desligado, também será substituído.

Para apagar as substituições (overrides), veja as seções [Mudando o Timeslot no modo DMR](#changing-timeslot-in-dmr-mode) e [Entrada Manual do número de TalkGroup](#manual-talkgroup-number-entry).

### Mudando a largura de banda no modo FM

- No modo FM, pressionar a tecla **Estrela** alterna entre largura de banda do canal entre 25kHz e 12.5kHz.

### Controlando a potência de transmissão (Tx power)

O firmware tem duas formas principais de controlar a potência de saída:

1. O controle de potência **Mestre** (Master), que controla a potência de ambos os VFOs, e também todos os canais.
2. Potência específica do **Canal**.

Por padrão, todos os Canais são configurados para usar o ajuste de potência **Mestre**, contudo, essa configuração pode ser modificada no CPS (e também na tela **Detalhes do Canal**), assim canais individuais podem ter sua própria configuração personalizada de ajuste de potência.

Quando um Canal tem um ajuste personalizado no nível de potência, a potência será mostrada em **Negrito**.

Aumentar ou baixar a potência em um canal com um ajuste personalizado irá temporariamente sobrepor a configuração de potência para o Canal, mas essa modificação não é salva para o codeplug. Assim, mudar de canal fará com que a alteração temporária na potência seja perdida.

Para fazer uma modificação **permanente** para o valor personalizado de potência do Canal, você deve abrir a tela [**Detalhes do Canal**](#channel-details), e então sair pressionando **SK2** + **Verde**.

Aumentar ou baixar o nível de potência em um Canal que usa o controle de potência **Mestre** irá mudar o nível de potência **Mestre** também **para todos os outros canais** que usam o ajuste de potência **Mestre** e ainda **ambos os VFOs**.

<div style="page-break-after: always; break-after: page;"></div>

Mudar a potência em **qualquer** VFO também muda o ajuste de potência **Master**.

- Pressione **SK2** + **Direita** para aumentar a potência.
- Press **SK2** + **esquerda** para diminuir a potência.

A potência pode ser ajsutada para **50mW**, **250mW**, **500mW**, **750mW**, **1W**, **2W**, **3W**, **4W**, **5W** e **+W-**.
O MD-9600 tem potência de saída maior e os ajustes de potência são diferentes.

O ajuste de potência **+W-** configura o drive do amplificador de potência (PA) para o valor especificado pela configuração "Potência do Usuário" no Menu de Opções.
Por padrão, esse valor é ajustado para o máximo possível. Isso fará com que o rádio produza a máxima potência que conseguir.
**O ajuste de potência que resulte no rádio dar mais potência do que é projetado para produzir deve ser usado com cautela, em emergências somente, uma vez que o uso extendido poderá danificar o PA**

Se o nível de Potência do Usuário for configurado para um valor muito pequeno, poderá ser utilizado para saídas de muito baixa potência, por exemplo, menos que 50mW.
Veja o menu de configuração da Potência do Usuário para mais informações.


Para acessar esse nível de potência, escolha o ajuste máximo de potência, então pressione e segure **SK2** + **Direita**

*Notas:*

- A potência de saída só será correta depois que o operador tiver calibrado seu rádio, porque esses rádios **não aparentam possuir uma calibração de potência muito precisa aplicada na fábrica**.
- A potência de saída em ajustes de **1W** ou abaixo **não são** muito precisas, porque a calibração só mantém pontos de dados para os valores de potência de **1W** e **5W**.
- Entre **1W** e **5W**, a potência do FET do PA é aproximandamente "diretamente proporcional" ao nível de drive do PA, por isso, os níveis de drive interpolados resultam em níveis de potência *razoavelmente precisos* para **2W**, **3W** e **4W**.
- However, below **1W** the PA FET output power **is not directly proportional** to the PA drive level, and **considerably varies** between different radios. Hence, the power accuracy below **1W** is at best around **80% accurate**.
- Além disso, o limiar operacional mínimo do FET do PA é muito próximo (ou às vezes até mesmo acima) de **50mW**, assim operar nesse nível de potência **pode produzir emissões espúrias indesejadas**.
- Por favor confirme sua potência de saída e emissões espectrais **antes** de usar o ajuste **50mW** em qualquer lugar, porque ele pode causar interferencia.

### Gráfico de barra de intensidade de sinal

Em ambos os modos FM e DMR, a intensidade de sinal do sinal recebido é mostrada como um gráfico de barra que de desloca pela largura da tela.

O gráfico de barra em **100%** é aproximadamente **S9 +40dB**.

No modo FM, o medidor de sinal deve operar durante todo o tempo.

![signal meter](media/signal-meter.png)

*Notas:*

- Atualmente, a leitura do S meter **não é** muito precisa porque a sensibilidade de Rx do hardware do rádio **não é calibrada** na fábrica.
- Por isso, o valor mostrado é baseado em um rádio com sensibilidade dentro da média. Rádios individuais podm ser **mais ou menos** sensiveis que a média, portantoo S meter irá mostrar **a mais ou a menos** do que é absolutamente correto.

### Funcionalidade específica da tela de Canal

A tela de Canal mostra o número do Canal atual, bem como a zona atual.

![channel and zone](media/channel-and-zone.png)

#### Mudando canais dentro da zona atual<!-- linebreak -->

- Pressionar as teclas de seta **Acima** ou **Abaixo** muda o Canal dentro da zona atual, e o número do Canal na zona será exibido ao lado do nome da zona.

#### Mudando zonas<!-- linebreak -->

- Pressionar **SK2** + seta **Acima** ou **SK2** + seta **Abaixo** muda para a próxima zona ou a zona anterior, respectivamente.

![another zone](media/changing-zones.png)

#### Mostrando a frequência do canal<!-- linebreak -->

- Pressione e segure o botão **SK1** para mostrar as frequências de Rx e Tx, tanto no modo DMR quanto no FM.


#### Exibindo informações espcíficas do canal FM<!-- linebreak -->

- Pressione e segure o botão **SK1** para mostrar informações específicas de FM: CTCSS / DCS e ajuste do silenciador.


#### Operação no reverso da repetidora<!-- linebreak -->

- Modo Canal: Pressione e segure a tecla **Grade** (#, também chamada cerquilha, hash, cruz, etc), e as frequências de Tx e Rx para o canal serão trocadas. O nome do canal será mostrado em vídeo reverso.
- Modo VFO: Pressione e segure **SK1** e **SK2** e as frequências de Tx e Rx serão trocadas.
- O rádio permanece bloqueado no modo reverso mesmo se o canal ou zona forem mudados.
- Para sair do modo reverso, pressione e segure **Grade**

*Nota:*

- Essa função é mutuamente exclusiva com a função [Talkaround](#talkaround) do Canal. Ou seja, ou usa o reverso ou o Talkaround, mas não ambos ao mesmo tempo.


#### Menu rápido do Canal<!-- linebreak -->

- Pressinar o botão **Laranja** no topo do rádio em modo Canal exibe o Menu Rápido para a tela de Canal. Note que no Menu Rápido, o botão **Laranja** tem a mesma funçãoda tecla **Verde**, que confirma sua seleção atual.

![channel quick menu](media/channel-quick-menu.png)

*Nota:*

- O Baofeng RD-5R e o MD-UV380 não tem um botão **Laranja**. 

No Baofeng RD-5R pressione e segure o botão de cor laranja **MR/VFO** para entrar no Menu Rápido.
No TYT MD-UV380 pressione **SK1** e o botão **Verde**

##### Copando um canal para o VFO<!-- linebreak -->

- Pressione o botão **Laranja** ou a tecla **Verde** para copiar o conteúdo do canal atual para o VFO.

##### Gravar o VFO no canal atual<!-- linebreak -->

- Pressione o botão **Laranja** ou a tecla **Verde** para confirmar e salvar o canal atualizado para a memória de codeplug. Tecla **Vermelha** para cancelar.


<div style="page-break-after: always; break-after: page;"></div>

##### Filtros<!-- linebreak -->

- **Filtros** no modo FM

  - Use as setas **Direita** ou **Esquerda** para ativar ou desativar os filtros CTCSS / DCS.

- **Filtros** no modo DMR

  - Use as setas **Direita** ou **Esquerda** para selecionar:

    - **Nenhum**: para não usar filtros, *por ex.* modo **promíscuo**.
    - **TG**: para filtrar pelo *Grupo de Conversa* (Talkgroup) selecionado.
    - **Ct**: para filtrar pelos *Contatos de Chamada Privada* (Private Call) no codeplug.
    - **TGL**: para filtrar pelos *Grupos de Conversa* na lista de TG.

  Quando o filtro estiver ativado, a indicação do modo *DMR* no topo da tela será exibida em vídeo reverso.

- **Varredura de CC** (*modo DMR somente*) (anteriomente conhecido como **Filtro CC**)

  Essa configuração permite que o rádio receba sinais mesmo quando o Código de Cor (Color Code, ou simplesmente CC) não seja conhecido.
  **Mas essa configuração atualmente não destativa o requerimento do CC**, porque o hardware, o chip HR-C6000, não suporta a recepção de sinais DMR sem um Código de Cor ser especificado.  
  Quando a funcionalidade de varredura (scanning) está ativada, é executada por um algoritimo de software, escrito por Colin G4EML, onde o valor do CC ajustado no HR-C6000 é modificado para cada frame DMR TS que é recebido, até que o HR-C6000 reporte que o CC do sinal de Rx do DMR é o mesmo CC que foi ajustado no HR-C6000.

  Esse recurso **NÂO DEVE** ser usado na operação normal. A detecção de CC é lenta, e pode fazer com que os sinais DMR nao sejam recebidos corretamente até que o CC seja encontrado pelo algorítimo.

  - Use as setas **Direita** ou **Esquerda** para ativar ou desativar.

  Quando a varredura de *Código de Cor* está ativa, o número *Color Code* é mostrado em vídeo reverso.

- **Filtro TS** (*modo DMR somente*)

  Controla se o rádio filtra por *Timeslot*.

  - Use as setas **Direita** ou **Esquerda** para ativar ou desativar.

  Quando o filtro de *Timeslot* está desativado, o número do *Timeslot* é mostrado em vídeo reverso.

  *Notas:*
  
  - Eesse recurso atualmente não desativa um filtro, porque o chip do hardare do DMR, HR-C6000, não suporta completamente a recepção de sinais em ambos os timeslots ao mesmo tempo.
  - Esse recurso usa um algoritimo de software, escrito por Daniel F1RMB, que inicialmente ouve os dados de ID do chamador em ambos os timeslots, e quando dados válidos ocorrem em um deles, o firmware simplesmente escuta nesse timeslot.
  - Se o ID do chamador não estiver presente no timeslot recebido por um período de timeout de aproximadamente 2,5 segundos, o algorítimo checa no outro timeslot e muda para ele se os dados de ID do chamador estiverem nesse timeslot.


##### Talkaround<!-- linebreak -->

Quando ativado, a frequência de TX será ajustada para a frequência de RX, assim você poderá transmitir na saída do repetidor, em modo simplex.

*Nota:*

- Essa opção somente está disponível se o Canal atual tiver um deslocamento nas frequências (shift).
- Essa opção é mutuamente exclusiva com a [Operação no reverso da repetidora](#reverse-repeater-operation).

##### Ordenar distância<!-- linebreak -->

Se o local do transceptor estiver definido (A tela de [Localização](#location-screen) em Informações do Radio ou GPS), a Zona atual será ordenada pela ordem de distância ascendente.

A distância, em quilômetros, é exibida à direita do nome da Zona.

É claro, para que isso funcione, a localização das repetidoras deve ser configurada nos canais relevantes, usando o CPS.

*Notas*:

- A zona "Todos os Canais" nunca será ordenada.
- A distância para o repetidor também pode ser mostrada sem ordenação, veja **Opções de Tela** [Mostra Distância](#show-distance).


<div style="page-break-after: always; break-after: page;"></div>

#### Menu Rápido do VFO<!-- linebreak -->

- Pressionar o botão **Laranja** no topo do rádio no modo VFO exibe o Menu Rápido para a tela do VFO. Atualmente, ele tem cinco opções.

![VFO quick menu](media/vfo-quick-menu.png)

*Nota:*

- O Baofeng RD-5R não tem um botão **Laranja**. Nesse rádio pressione e segure o botão laranja **MR/VFO** para entrar no Menu Rápido

##### Seleção de VFO A ou B<!-- linebreak -->

- Pressionar o botão **Laranja** duas vezes enquanto no modo VFO muda rapidamente entre o **VFO A** e o **VFO B**.
- No Baofeng DM-1801 | DM-860, essa função é controlada usando o botão **A/B**.
- **Pressionamento Longo** do botão **Vermelho** também muda do VFO A para o VFO B, ou vice versa.

##### Trocar as frequências de TX e RX<!-- linebreak -->

Essa função essencialmente inverte as frequências de TX e RX.

- Pressione a tecla **Verde** ou o botão **Laranja** para confirmar.

##### Copiar a frequência de RX para a frequência de TX<!-- linebreak -->

Copia a frequência de Rx para a frequência de Tx.

- Pressione a tecla **Verde** ou o botão **Laranja** para confirmar.

##### Copiar a frequência de TX para a frequência de RX<!-- linebreak -->

Copia a frequência de Tx para a frequência de Rx.

- Pressione a tecla **Verde** ou o botão **Laranja** para confirmar.

##### Filtro (*DMR mode only*)<!-- linebreak -->

Essa função é identica ao Filtro descrito para a operação no modo Canal ([acima](#filter))

##### VFO para Novo Canal<!-- linebreak -->

A opção **VFO --> Novo Canal**, cria um novo canal usando as configurações atuais do VFO.

O nome do novo canal usa o formato "**New channel** *NNN*", onde *NNN* é o próximo número disponível na zona *Todos os Canais*.

O canal também será adicionado na Zona atual ativa, na tela de Canal. Se a tela de Canal estiver ajustada para a zona *Todos os Canais*, o canal será adicionado a essa zona.

##### Varredura de subtom (Tone Scan) para tom CTCSS ou DCS em FM<!-- linebreak -->

Essa varredura procura qualquer tom **CTCSS** ou **DCS**, e ajusta o VFO para esses parâmetros.

O padrão é procurar por **Todos** os tons (CTCSS e DCS). Para procurar por CTCSS ou DCS somente, pressione as teclas de seta **Direita** ou **Esquerda** para selecionar **CTCSS** ou **DCS**.

- Pressione o botão **Laranja** ou a tecla **Verde** para confirmar a seleção, ou a tecla **Vermelha** para cancelar.

Cancelar a varredura restaura o CTCSS / DCS de Rx para o valor de antes da verredura ser iniciada.

Se um tom for detectado, ambos os valores de Rx e Tx do CTCSS / DCS são ajustados para o tom que foi detectado pela varredura.


<div style="page-break-after: always; break-after: page;"></div>

### Funcionalidade específica do DMR (telas *VFO e Canal*)

#### Seleção de Timeslot<!-- linebreak -->

- A tecla **Estrela** alterna entre *TimeSlot 1* e *TimeSlot 2*.

#### Exibição de indicativo DMR ID e nome<!-- linebreak -->

Qaundo um sinal DMR é recebido que usa o mesmo *Código de Cor*, como selecionado para o Canal ou VFO, a tela do rádio irá mostrar o **Talkgroup** e **DMR ID** da estação.

![talkgroup and DMR ID](media/talkgroup-and-dmr-id.png)

Se o ID do DMR estiver no *Banco de dados de DMR ID*, previamente carregado no rádio, o **indicativo** e o **nome** serão mostrados.

![callsign and name](media/callsign-and-name.png)

#### Exibição de Talker Alias<!-- linebreak -->

Se receber um sinal da rede *Brandmeister*, e se o DMR ID da estação não estiver no *Banco de dados de DMR ID* do rádio, a tela mostrará a informação **Talker Alias** enviada pela rede *Brandmeister*.

![talker alias](media/talker-alias.png)

O indicativo será mostrado no centro da tela, e as informações adicionais na parte de baixo. A informação adicional por padrão será o texto "**DMR ID:**" seguido pelo número de identificação (ID) da estação **Número do DMR ID**.


<div style="page-break-after: always; break-after: page;"></div>

Se a estação tiver entrado quaisquer dados na **Seção APRS** da página “*Self care*” da Brandmeister dela, esse texto será mostrado no lugar do número DMR ID.

![talker alias data](media/talker-alias-data.png)

*Nota:*

- Como os dados de **Talker Alias** são enviados lentamente por serem embutidos dentro dos frames de áudio do DMR, o indicativo aparecerá primeiro, e depois de aproximandamente meio segundo, o DMR ID ou outro texto chegará via dados DMR e será mostrado.

#### Seleção de Grupo de Conversa (Talkgroup) da lista de TG<!-- linebreak -->

Pressione as teclas de seta **Esquerda** ou **Direita** para percorrer os *TalkGroups* na **Lista de TG** (TG List) atribuídos ao VFO ou Canal pelo CPS.

Esse *TalkGroup* será aplicado a **ambos** RX e TX.

- Se um canal não tiver uma *Lista de TG* atribuída, o Contato atribuído ao Canal será usado, e as setas **Esqerda** e **Direita** não terão efeito.
- Se um canal não tiver uma *Lista de TG* atribuída, e o Contato estiver definido como **Nenhum** ou **N/A**, o rádio vai usar por padrão o **TG 9**.

*Nota:*

- O Baofeng RD-5R não tem teclas de seta **Direita** e **Esquerda**. Use o botão **A/B** como seta esquerda e o botão **Band** como seta direita.

#### Atribuição de Timeslot ao Grupo de Conversa do Contato Digital<!-- linebreak -->

Um novo recurso introduzido no CPS permite um *TimeSlot* padrão ser aplicado a cada **Contato Digital** ou **Grupo de Conversa**.

Por padrão, a **Substituição de TS do Canal** é desativada. Isso significa que se as setas **Esquerda** ou **Direita** forem pressionadas para selecionar o **TG** dentro da *Lista de TG*, o *Timeslot* atribuído ao Canal (*no CPS*) ou mudado manualmente usando a tecla **Estrela** não mudará.

Contudo, se o **Contato Digital** tem uma **substituição de TS** atribuída (*por ex.* TS 1), quando o **TG do Contato Digital** for selecionado pelas setas **Direita** ou **Esqeurda**, o *Timeslot* será ajustado para aquele atribuído ao **TG do Contato Digital**.  
Nesse caso, o Timeslot é mostrado como **cS***x* nas telas Canal/VFO (cS1 nesse exemplo).


<div style="page-break-after: always; break-after: page;"></div>

#### Grupo de Conversa mostrado em video reverso<!-- linebreak -->

Se um *Talkgroup* for mostrado em vídeo reverso durante a recepção de um sinal DMR, isso indica que o Grupo de Conversa de TX (*TX TalkGroup*) **não combina** com o *TalkGroup* recebido, por isso pressionar **PTT** não irá transmitir de volta para a estação no mesmo *TalkGroup*.

![talkgroup in inverse video](media/talkgroup-inverse-video.png)

Se você quiser transmitir no mesmo Grupo de Conversa (*TalkGroup*) do sinal atualmente recebido, pressione o botão **SK2** do lado do rádio **enquanto** o *TalkGroup* estiver sendo mostrado em vídeo reverso. O *TX TalkGroup* será então ajustado para o *RX TalkGroup*.

![talkgroup temporary set](media/talkgroup-override.png)

#### Entrada manual do número do Grupo de Conversa (TG)<!-- linebreak -->

- Pressione a tecla **Grade** (**#**) para entrar um número de TalkGroup via método *ad hoc*, ou seja, entrar o número de TG diretamente, seguido da tecla **Verde** para confirmar.

![talkgroup entry screen](media/talkgroup-entry.png)

Se o **TG** entrado estiver nos *Contatos Digitais*, o nome do **TG do Contato** será mostrado, caso contrário o número será mostrado. *por ex.* **TG 98977**.

- Para retornar ao *TG* anterior que estava antes de de entrar manualmente o TG, pressione as teclas de seta **Esquerda** ou **Direita**.

Quando um *TG* foi **entrado manualmente**, a tela mostra uma caixa com **1 pixel de espessura** ao redor da área de exibição do TG para indicar que esse TG foi digitado manualmente, mesmo se o *Contato / Nome do TG* for mostrado ao invés do número.

![talkgroup override](media/talkgroup-manually-entered.png)

#### Entrada de número de Chamada Privada (Private Call)<!-- linebreak -->

- Pressione a tecla **Grade** (**#**) duas vezes para entrar um número de ID do DMR para chamada privada.

![personal DMR ID entry screen](media/private-call-entry.png)

Em todas as telas de entrada numérica, pressionar a tecla de menu **Vermelha** volta para a tela anterior, seja a tela de VFO ou Canal.

#### Seleção de Contato Digital<!-- linebreak -->

- Pressione a tecla **Grade** (**#**) três vezes para acessar os Contatos Digitais definidos no CPS.

![contact selection screen](media/contact-selection.png)

O nome do contato é mostrado no meio da tela, *por ex.* “**TG 505 TS2**” e o número do *TalkGroup* ou Contato Pessoal (*PC*) é mostrado em texto menor na parte de baixo da tela.

- Pressione as setas **Acima** ou **Abaixo** para percorrer a lista de *Contatos Digitais*.
- Pressione **Verde** para selecionar ou **Vermelho** para cancelar.

Chamadas Privadas também podem ser selecionadas dessa maneira.

![private call selection](media/private-call-selection.png)

#### Entrada de número DMR ID da estação<!-- linebreak -->

- No **Modo de seleção de Contatos**, pressione as teclas **SK2** + **Grade** (**#**). Um **DMR ID** *alternativo* pode ser entrado no rádio (*para propósito de testes*) de forma a substituir temporariamente seu número de DMR ID normal, que foi carregado pelo codeplug.

![DMR ID entry screen](media/user-dmr-id.png)

Esse DMR ID será usado para a transmissão **até que o rádio seja reiniciado**, ou você entre outro DMR ID pela mesma tela.

Para tornar a modificação permanente, de forma que seja salva de volta no codeplug, pressione **SK2** + **Verde** ao invés de **Verde** para confirmar o número.


<div style="page-break-after: always; break-after: page;"></div>

### Funcionalidade específica de FM (*Telas VFO e Canal*)

#### FM e FM Faixa estreita (Narrow)<!-- linebreak -->

Para FM com **25kHz de largura de banda**, o texto “**FM**” é mostrado no canto superior esquerdo da tela. Já para faixa estreita com **12.5kHz de largura de banda**, o texto “**FMN**” é exibido.

#### Tom CTCSS ou Código DCS<!-- linebreak -->

Esses podem ser configurados para o Chanal ou o VFO. AS letras **C** ou **D** e **T**, **R**, ou **TR** serão mostradas próximo ao indicador FM no topo da tela.

![CSS status](media/ctcss-tone.png)

**C** significa CTCSS, **D** significa código DCS. **T** indica tom (ou código) somente no Tx. **R** indica tom (ou código) somente no RX. **TR** significa que os tons (ou códigos) foram configurados tanto em Tx quanto em Rx.

É possível configurar tons ou códigos em Tx e Rx independentemente.

#### Silenciador (Squelch)<!-- linebreak -->

- Pressionar as teclas **Esquerda** ou **Direita**, controla o silenciador em FM.

![squelch level](media/squelch.png)

Dentro do modo de controle do silenciador, pressionar **Direita** fecha o squelch incrementalmente, **Esquerda** abre o squelch incrementalmente. O VFO e cada canal tem configurações individuais de silenciador que podem ser ajustadas dessa forma.

O silenciador variável pode ser ajustado para valores diferentes para cada Canal e para o VFO usando um novo recurso no CPS, onde o squelch pode ser ajustado em qualquer posição entre **Aberto** e **Fechado** em **passos de 5%**.

Nesse exemplo o squelch do VFO está ajustado para 20%.

Se o silenciador for mudado no VFO, o valor será lembrado mesmo que o rádio seja reiniciado. Contudo, se o silenciador de um canal for mudado, o valor é só uma substituição temporária.

Para tornar as mudanças no squelch permanentes para um Canal, pressione **SK2** + **Verde** para entrar na tela de *Detalhes do Canal*, e então pressione **SK2** + **Verde** novamente para salvar os dados do canal para o codeplug.

*Nota:*

- Se o CTCSS de Rx estiver ativado, tem prioridade sobre o controle do silenciador, e baixar além do nível de limiar não fará com que o squelch seja aberto.

#### Tom de 1750Hz para operação em repetidora<!-- linebreak -->

- Pressionar o botão **SK2** durante a transmissão em FM envia o tom de 1750Hz requerido para operação em algumas repetidoras.

#### Transmissão de tom DTMF<!-- linebreak -->

- Pressionar qualquer tecla no teclado frontal (exceto as teclas de menu **Verde** e **vermelha**) durante a transmissão fará com que sejam transmitidos os tons DTMF para essa tecla.

O tom também será audível através do alto-falante no GD-77, RD-5R, DM-1801 e DM-1801A.
No MD-UV380 e MD-9600, um tom é emitido atráves do alto-falante. Mas esse não é o tom DTMF que é transmitido, porque o hardware desses rádios não suporta tocar os tons DTMF reais através do alto-falante.

Os botões do microfone do The MD-9600 para A, B, C e D já são usados para outras funções. Por ex. A = botão vermelho/ESC, assim as seguintes sequências de tecla precisam ser usadas para entrar as letras A, B, C e D:

| **Tecla(s)** | **DTMF** |
| --- | --- |
| **Acima** | A |
| **SK1** + **Acima** | B |
| **Abaixo** | C |
| **SK1** + **Abaixo** | D |

*Nota:*

- Atualmente a versão do firmware do MD-9600 não pode transmitir CTCSS ou DCS ao mesmo tempo com o DTMF

#### Entrada de sequência DTMF e transmissão<!-- linebreak -->

- Pressione a tecla **Grade** (**#**) para entrar uma sequência DTMF (pressionar SK2 + Esquerda deleta um caracter)

![dtmf entry screen](media/dtmf-sequence-entry.png)

- Pressionar **SK2** + **Grade** (**#**) alterna entre as telas de entrada DTMF e a lista de contatos DTMF.
  
![dtmf contact list screen](media/dtmf-contact-list.png)

- Pressione a tecla **Verde** para transmitir essa sequência.
- Qualquer tecla pressionada irá interromper a transmissão da sequência atual.

#### Transmissão da localização FM APRS<!-- linebreak -->

O firmware pode transmitir dados em FM da rede Automatic Packet Reporting System (APRS), como uma transmissão FM AFSK 1200 baud ou 300 baud, seja usando o local entrado no rádio, ou usando a localização GPS para os rádios com GPS instalado.

Veja [https://pt.wikipedia.org/wiki/APRS](https://pt.wikipedia.org/wiki/APRS)

Para transmitir APRS, pelo menos uma configuração APRS deve ser definida usando o CPS, e o canal atual ou VFO deve ter uma configuração APRS selecionada (veja Configurações APRS em Detalhes do Canal).
Também é necessário que o indicativo do operador seja entrado no CPS, e a localização do rádio esteja válida, seja por entrada manual do local, ou pelo uso do GPS no rádio, se instalado.


Also, the beaconing mode as to be defined (see the [APRS Options](#aprs-options))

In **Manual** mode is selected, you will have to press **SK1** + **2** key, while in **Channel** in **VFO** screen, to transmit a beacon.
In **PTT** mode, a beacon is send when releasing the **PTT** key, which permits voice transmission (bear in mind that the **Interval** and **Decay** beaconing settings re honored here too).

When APRS beaconing is used in Satellite screen, and APRS Tx/Rx frequency is selected, pressing the PTT key will immediately send a beacon, regardless of the **Interval** and **Decay** settings.

In some radios there is audio feedback through the speaker to indicate that the packet is being set, but this is not currently supported on all radios, specifically not on the MD-9600 or DM-1701 due to hardware limitations.

If the location data is not valid in **Manual** or **PTT** beaconing modes, the word "Location?" will be displayed on the screen and the data will not be transmitted. In automatic modes (**Auto** and **Smart**), no beacon will be transmitted until a valid location is set (in [Location screen](#location-screen) screen or having a GPS fix on featured transceivers). 

The CPS allows up to 8 APRS configurations to be defined. With multiple parameters including specifying the Icon to be displayed on sites like https://aprs.fi and also the Comment text.



*Notes:*

- Currently only APRS Tx is supported. It is currently unknown whether the hardware in any of the supported radios can be used to receive APRS or other AX25 packet transmissions.
- Voice communication is not possible on a channel or VFO which has an APRS configuation selected.
- The APRS packet data format only allows for up to 6 character callsigns. This is a limitation of the specification not the firmware.
- Satellites have specific APRS parameters which need to be used, so default APRS parameters are defined in the satellites data uploaded from the CPS. To override these parameters, define an APRS config with the same name as the satellite, and set the appropriate custom parameters you wish to use with that satellite
- Most VHF and UHF APRS systems use 1200 baud



<div style="page-break-after: always; break-after: page;"></div>

### VFO specific functionality

The VFO displays both the TX and RX frequency at all times.

![VFO screen](media/vfo-screen.png)

When the currently selected frequency is the **RX** frequency, an arrow (**\>**) is displayed to the left of the “**R**”, changes to the frequency will adjust both the TX and RX frequencies.

#### Frequency change up/down step<!-- linebreak -->

- Pressing the **Up** or **Down** arrows will change frequency by the frequency step value defined for the VFO in the CPS.

The step can be adjusted by pressing **SK2** + **Green** to enter the Channel Details mode, and then adjusting the “**Step**” setting

#### Numerical frequency entry<!-- linebreak -->

- Pressing **any of the number keys** allows the direct entry of the frequency.

![frequency entry screen](media/frequency-entry.png)

When all digits have been entered, the accept beep tones are played, and the display returns to the VFO screen.

If an invalid frequency is entered the error beep tones are played.

When entering a frequency:

- Pressing the **Red** key cancels the entry.
- Pressing the **Left** arrow deletes the digits one by one.

#### To adjust the TX frequency, independent of the RX frequency<!-- linebreak -->

- Press and hold **SK2** button on the side of the radio, and then the **Down** arrow.

This will change the currently selected frequency to the TX frequency, and the arrow will move to the left of the “**T**” instead of the “**R**”

To change the RX frequency again, press **SK2** + **Up** arrow.

When the TX frequency is changed, the RX frequency will not be changed.

Use this method to set different TX and RX frequencies. For example, this can be useful for satellite operation as it allows **Cross Band** operation as well as **Split** frequency simplex operation on the same band.

*Note:*

- If different TX and RX frequencies are set, and the currently selected input is set to RX, changing the RX frequency will also change the TX frequency, and the difference between the RX and TX frequency will be maintained if possible.

The only case where the frequency difference **will not be maintained** is if the TX frequency goes outside the range of frequencies supported by the radio hardware.

#### Spectrum sweep scan<!-- linebreak -->

- Press and hold the **Hash** # key to enter Spectrum sweep scan mode.

The radio then starts scanning a band of frequencies centered on the current Rx frequency, and displays the signal strength in the forum of a spectrum amplitude graph.
The bandwidth of the scan is shown in the top left corner of the display e.g. +/- 800kHz

  - **Left** / **Right** : Step down or up central frequency of sweep
  - **SK2 + Left** / **SK2 + Right**: Change overall sweep bandwidth aka zoom
  - **Down** / **Up**: Decrease / increase virtual gain
  - **SK2 + Down** / **SK2 + Up**: Decrease / Increase virtual noise floor
  - **SK1 + Up** or **SK1 +Down**: Resets the gains/floor to default

Monitor mode (long press on **SK2**) suspends the scan and open the receiver to the central frequency.

![Spectrum scan](media/vfo-spectrum-scan.png)

#### VFO Dual Watch<!-- linebreak -->

In the VFO Quick Menu, select Dual Watch

In this mode, the radio will scan the VFO A and VFO B frequencies.
In this mode rather than displaying the Rx and Tx frequency of an individual VFO, the Rx frequency of VFO A and VFO B is displayed.
While scanning in this mode, the FM/DMR mode area of the screen, flashes the [DW]
To exit Dual Watch press any key.

*Notes:*

- VFO Dual Watch, functions in the same way as the Zone scan in Channel mode.
- Both VFO A and VFO B have equal priority. Once the scan has stopped on one VFO, because there is a signal, the scan does not sample the other VFO to determine if it also has a signal.
- VFO A and B do not need to both be FM or both be DMR. Either VFO A or B can be either FM, FM Narrow or DMR mode.


#### Easily changing from VFO A to VFO B, and vice versa<!-- linebreak -->

An alternative method to change the current VFO, is to **Long Press** on the **Red** key.


<div style="page-break-after: always; break-after: page;"></div>

## Monitor mode

Monitor mode enables the operator to listen to a signal even if it is currently being filtered by either the **DMR TG**, **TS** or **CC** filters or the **FM CTCSS / DCS** filter or **FM squelch** level setting.

- To enable Monitor mode press and hold button **SK2** button (which is the **SK2** button on the GD-77).

After 2 seconds the radio will enter monitor mode, and stay in this mode until the **SK2** is released.

When Monitor mode is active:

- In **FM mode**: any Rx **CTCSS / DCS** filter is disabled, and the squelch is changed to be fully open.
- In **DMR mode**: the **TG**, **TS** and **CC** filters are disabled, and if **no DMR signal is detected within 250mS** the radio is switched to FM mode with the CTCSS / DCS and squelch disabled.

Releasing the **SK2** button returns the radio back into the mode and filter configuration prior to it being pressed.


<div style="page-break-after: always; break-after: page;"></div>

## Transmitting

During transmission the *Talk Timer* either counts up or down, depending on whether the channel has a timeout defined.

If a timeout is defined in the CPS, or adjusted in the *Channel Details* screen, the *Talk Timer* will count down and when the timeout period is reached a beep will play and the TX will stop.

In **DMR Tier2** the timer will not start counting until the repeater becomes active.

During FM and DMR Tx, a *VU meter* is displayed showing the input microphone level, in the form of a bar graph across the top of the screen.

![VU meter](media/dmr-mic-level.png)

### Timeout warning beep

A timeout warning can be configured in the **Sound Options** menu. The radio will beep every 5 seconds when the remaining call time is less than the timeout.

### TOT

If **TOT** is set up for the current Channel or VFO, when the timer counts down to zero, a warning beep will be played and the radio will stop transmitting.

![timeout screen](media/timeout.png)


<div style="page-break-after: always; break-after: page;"></div>

## Scanning

Both the Channel and VFO screens support scanning, but their operation is slightly different.

### Channel scanning

- Press and hold (**Long press**) the **Up** arrow to start scanning the channels in the zone. On the MD-9600 press and hold the **Up** arrow on the front panel of the radio.
- Press the **Left** arrow to reverse the direction of scan. Press the **Down** arrow on a MD-UV380 | RT-3S, or the one on the front panel for a MD-9600 | RT-90 (or **C** mic button), to reverse the scan direction.
- Press the **Right** arrow to mark the channel as a *nuisance* channel which will be removed from the current scan (or **B** on the microphone for a MD-9600 | RT-90). Press the **Star key** on a MD-UV380 | RT-3S.
- Press the **Up** arrow to skip over the current channel, and continue the scan. On the MD-9600 rotate clockwise the rotary knob on the front panel of the radio, or the **Up** arrow on the mic.

Pressing any other button stops the scan.

Whilst scanning, the mode indicator **DMR** or **FM** will flash.

### VFO scanning

The VFO screen has a special scanning mode, which is entered by performing a **Long Press** on the **Up** arrow button.

When scan mode is enabled, the display changes to show the *lower* and *upper* scan limit frequencies, instead of showing the Tx frequency.

Initially the scan limits will be set to the current VFO Rx frequency, minus 1Mhz to plus 1Mhz.

Scan limits can be changed by manually entering both frequencies *e.g.*

**1 4 4 0 0 0 1 4 8 0 0 0**

- To start the scan, use Long press on the **Up** arrow, until the radio beeps.

When not actively scanning, pressing the **Up** or **Down** arrows performs the normal function in the VFO of increasing or decreasing the frequency.

- Press the **Left** arrow key to reverse the scan direction. Press the **Down** arrow on a MD-UV380 | RT-3S, or the one on the front panel for a MD-9600 | RT-90 (or **C** mic button), to reverse the scan direction.
- Press the **Up** arrow to skip over the current frequency and continue the scan. On the MD-9600 rotate clockwise the rotary knob on the front panel of the radio, or the **Up** arrow on the mic.
- Press the **Right** arrow to mark the current frequency as a *nuisance* frequency, which will be omitted by the scan (or **B** on the microphone for a MD-9600 | RT-90). Press the **Star key** on a MD-UV380 | RT-3S.

Pressing any other button will stop the scan

- Long press on the **Down** arrow arrow exits from scan mode.


<div style="page-break-after: always; break-after: page;"></div>

## Other screens

### Lock screen

To lock the keypad.

![keypad lock screen](media/lock-screen.png)

On either the VFO or the Channel screen, press the **Green** menu key to display the **Main menu**, then press the **Star** key. Pressing the **Star** key from any top-level item within the Main menu locks the keypad.

- To unlock the keypad, press and hold the **SK2** button and press the **Star** key.

You can also lock the **PTT** button by pressing the **Green** menu key to display the Main menu and then pressing the **Hash** (**#**) key. The keypad **and** the **PTT** can both be locked at the same time by first locking the **PTT** and then the keypad.

![full lock screen](media/keypad-and-ptt-locked.png)

### Text entry

The firmware now supports alphanumeric text entry while creating a new contact or editing an existing one.

![alphanumric entry](media/text-entry.png)

- Press **Left** and **Right** to move the cursor.
- Press **SK2** + **Left** to backspace, and **SK2** + **Right** to insert a space.

The keypad entry follows the same functionality as stock GD77 firmware.


<div style="page-break-after: always; break-after: page;"></div>

## The control keys and buttons

![GD-77 cheatsheet](media/RadioButtonsHSs.jpg)<!-- { width=600 } -->

![DM-1801 cheatsheet](media/DM-1801-Cheatsheet-01.svg)<!-- { width=600 } -->

![RD-5R cheatsheet](media/RD5R-CheatSheet.png)<!-- { width=600 } -->

![MD-9600 cheatsheet](media/MD9600-CheatSheet.png)<!-- { width=600 } -->

![MD-UV380 cheatsheet](media/MD-UV380-CheatSheet.png)<!-- { width=600 } -->


<div style="page-break-after: always; break-after: page;"></div>

## The Menu System

The firmware has its own menu system, which is completely different from the official firmware.

Targeted at amateur use, this focuses on being more straightforward, with highlight on commonly-used features.

Please refer to the menu map below.

![](media/menu-roadmap-1.png)

![](media/menu-roadmap-2.png)

![](media/menu-roadmap-3.png)

- Pressing the **Green** key enters the menu system, press again to enter a menu subsection or to exit the menu.
- Press the **Red** key to step back one level or to exit the menu system.
- The **Up** and **Down** arrow keys step up and down through the various pages of the menu system.
- The **Left** and **Right** arrow keys will change the individual items in the menu system where they are changeable.
- The **Blue** button on the side of the radio, known as **SK2**, is used as a **Function** key. Various features are accessed by holding the **Function** key when pressing a button on the keypad.
- Press the **Orange** button to access the quick menu from the standby screen.


<div style="page-break-after: always; break-after: page;"></div>

## QuickKeys

Individual menu screens scan be accessed quickly using the QuickKeys system.

Menus are assigned a QuickKey number, by entering the menu in question and pressing button **SK2** and any number key at the same time.

On the VFO or Channel screen pressing the same key e.g. **SK2** and "2" will open the same menu again.

QuickKeys can also be used to set individual settings in menus. Pressing **SK2** and any number key, on an individual setting, will display arrows to the left and right and the text "OK"

Pressing "OK" using the **Green** button, would create a QuickKey to an individual setting, but would not change it.

Pressing the **Left** or **Right** arrow keys, store a QuickKey which will decrease or increase the setting in question.

![quickkey setting assignment](media/quickkey_individual_setting.png)

Using a QuickKey which decreases or increases a setting, shows special screen displaying the setting that has been changed and its new value.

![quickkey setting action](media/quickkey_action_individual_setting.png)

To reassign a QuickKey to a different menu, it must first be cleared. On either the VFO or Channel screen, press and hold **SK2** and the number key in question, and wait for the beep sequence to play, to indicate the QuickKey has been cleared.

*Note:*

- QuickKeys can't be activated inside a menu, they can only be used on the VFO or Channel screen, and can only be assigned to menus or menu items.


<div style="page-break-after: always; break-after: page;"></div>

## Main Menu

![main menu](media/main-menu.png)

### Zone

This menu is used to select which groups of Channels, called a **Zone**, is used in the *Channel screen*, and operates in the same way as the official Radioddity firmware, except with one addition.

![zone list](media/zones.png)

In addition to the Zones that are defined in the CPS and uploaded to the radio using the CPS, the firmware creates a special Zone called **All Channels**.

![all channels zone](media/all-channels.png)

When the *All Channels* zone is selected, the Channel screen displays **All Channels** and the channel number instead of the Zone name and Channel number.

![all channel is selected](media/all-channels-channel-screen.png)

- Pressing the **Up** and **Down** arrows will cycle through all channels in the zone.
- Pressing any of the number keys on the keypad, enters **Goto** *channel number* mode.

![goto 12 is entered](media/goto-channel-number.png)

In this mode, you can enter multiple digits and then press the **Green** key to confirm, or the **Red** key to cancel.

Note that you can quickly cycle through zones by holding the **SK2** button and pressing **Up** or **Down** in *Channel mode*.

### RSSI

Displays a signal strength indicator showing the numerical **RSSI** value in **dBm**, along with an *S-Unit bar graph*.

![RSSI screen](media/rssi.png)

*Notes:*

- Both RSSI and S-meter are not calibrated and will vary somewhat between different radios in their accuracy.
- DMR signals by their nature, because they are pulse transmissions, **will not** give accurate RSSI values.

*The number in the top right of the display is for debugging purposes and is the number reported by the receiver hardware.*


<div style="page-break-after: always; break-after: page;"></div>

### Radio info

Displays various information about the status of the radio.

#### Battery voltage and percentage<!-- linebreak -->

This shows battery voltage and percentage.

![battery status screen](media/battery.png)

Press and hold the **SK2** button to display the *pure* battery voltage (non averaged value).

![pure battery voltage](media/pure-battery.png)

&rarr; Press the **Down** key to display the next page.

#### Time clock<!-- linebreak -->

Displays the time in either UTC or Local time, depending on the Display Options Time: setting.
To set the clock enter the full time in 24 hour time including all hours minutes and seconds, and press the **Green** menu key.

![realtime clock](media/radioinfo-time.png)

If using Local time. **You MUST set the Timezone before setting the time**

*Notes:*

- The clock only keeps time when the radio is turned on, or in Suspend Mode.
- The time accuracy varies from radio to radio, but can be accurate to approximately 5 second per day.
- Problems with time accuracy can be partially corrected by using the Time Cal: setting in the Options menu

&rarr; Press the **Down** key to display the next page.

#### Date screen<!-- linebreak -->

This displays and allows the entry of the date in either UTC or Local time, depending on the Display Options Time: setting.
To set the date enter the full date in format YYYY MM DD (Year Month Day), and press the **Green** menu key.

![date](media/radioinfo-date.png)

If using Local date / time. **You MUST set the Timezone before setting the date **

&rarr; Press the **Down** key to display the next page.

#### Location screen<!-- linebreak -->

This displays and allows the entry of the location in Latitude / Longitude

![location](media/radioinfo-location.png)

This screen is currently only used for the Satellite functionality.
But may be used in the future to send APRS data.

Enter the full Latitude / Longitude in DD.DDD DDD.DDD format (D degrees)

To change southern / northern hemisphere, press **Down** / **Up**
To change western / eastern hemisphere, press **SK2** + **Down** / **Up**

Before the location is set, this screen will display the message "NOT SET" and show question marks in place of the Lat / Long value

&rarr; Press the **Down** key to display the next page.

#### CPU temperature<!-- linebreak -->

This displays the CPU temperature in Celsius.

![temperature screen](media/temperature.png)

&rarr; Press the **Down** key to display the next page.

#### Battery voltage history<!-- linebreak -->

This shows the history of battery voltage on an hourly basis.

![battery history graph](media/battery-graph.png)

&rarr; Press the **Down** key to display the next page.

### Contacts

![contacts menu](media/contacts-menu.png)

#### DMR Contacts<!-- linebreak -->

Allows selection, Editing or Deletion of DMR Contacts

#### FM DTMF Contacts<!-- linebreak -->

Allows selection, Editing or Deletion of FM DTMF Contacts

#### New Contact<!-- linebreak -->

Allows a new DMR Contact to be created

### Last Heard

![last heard screen](media/last-heard.png)

Displays a record of the last 32 DMR stations that the radio has received.

- Pressing the **Up** or **Down** arrows cycles through the list to show stations which have been heard.
- Hold **SK2** button to view details like TalkGroup and time elapsed.
- Pressing the **Green** key will set the selected talkgroup as the new TG.
- Pressing the **Green** key, while **SK2** button is held down, will set the selected station DMR ID as the new PC / TG contact.
- Long press the **Hash** (**#**) key clears the list.

### Firmware Info and credits

![firmware info screen](media/firmware-info.png)

Displays the date and time the firmware was built, and also the GitHub commit code in brackets on the first page

To view details on GitHub, append the code to <https://github.com/rogerclarkmelbourne/OpenGD77/commit/>

*e.g.* <https://github.com/rogerclarkmelbourne/OpenGD77/commit/a0ebbc7>

Press **Down** to access the multiple credits pages

![credits screen](media/credits.png)

Details of the creators of firmware, current and past developers who have made major contributions to the firmware.

*Note:*

It's not practical to list every person who has helped with the development of the firmware.


<div style="page-break-after: always; break-after: page;"></div>

### Options

![options menu](media/options.png)

#### General Options

This menu controls various settings specific to the firmware

##### Key long<!-- linebreak -->

This setting controls the time (*in seconds*) after which a key is considered to be a long/repetitive press.

##### Key rpt<!-- linebreak -->

This setting controls the speed of key repetitions when a key is held.

##### Auto lock<!-- linebreak -->

This setting enables keypad/PTT auto-locking.

While in Channel or VFO screen **only**, and no user action has been made by the operator within the selected amount of time, the **PTT** and **keypad** keys will be locked (see [Lock screen](#lock-screen) to unlock).

Possible values: from 0.5 minute up to 15 minutes, with a step of 30 seconds.

*Note:*

- This doesn't interfere with scanning.


##### Hotspot<!-- linebreak -->

  - **Hotspot mode is not supported on the Baofeng RD-5R | DM-5R because the hardware does not support reliable USB communications while the radio is transmitting**

This option controls whether the firmware will enter hotspot mode when connected to MMDVMHost, including Pi-Star, or to BlueDV.

Options are:

- **Off**
- **MMDVM**: for use with Pi-Star or any other system using MMDVMHost.
- **BlueDV**: for use with BlueDV.

On the GD-77S. To enable hotspot mode, Press and hold the **SK1** (**Black**) button while turning on the radio. This will toggle hotspot mode between **MMDVM** and **BlueDV** mode.

##### Temp Cal<!-- linebreak -->

This setting allows the internal CPU temperature sensor to be calibrated by the operator.
The range is +/- 10 deg C in 0.5 deg C steps.

*Note:*

- The temperature value is the value measured by the CPU its self. It's not the temperature of the PA or the radio as a whole.

##### Batt Cal<!-- linebreak -->

This setting allows value of the voltage display to be calibrated.
The range is +/- 0.5V.

*Notes:*

- The battery voltage measurement is taken by the CPU from the internal battery voltage rail, and can differ from the value measured on the external charging terminals of the battery, especially when the radio is transmitting.
- Changing this calibration will affect both the voltage and percentage display.

##### Time Cal<!-- linebreak -->

This setting allows some calibration of the time clock which is maintained while the radio is turned on.
The range is +/- 7, the units are x / 10000, so a value of 1 results in a change of 1 second in 10,000 seconds.

The clock is currently an experimental feature and is not guaranteed to be accurate.

##### Eco Level<!-- linebreak -->

This setting controls the Economy or Rx Power Saving, operation of the radio.
The range is 0 to 5.
Rx power saving is achieved by pulsing the Rx and other parts of the internal electronics of the radio Off for small amount of time, to reduce current consumption and hence increase battery life.
The minimum setting is 0, which disables the Rx power saving and results in the Rx and all other electronics in the radio being powered on continuously.
The default setting is 1, which uses a 1:1 duty cycle. With an overall duty period of 240 milliseconds. 120 milliseconds On, 120 milliseconds off. In this Eco Level, power saving does not start until the radio had been idle for 10 seconds.

This table shows the values for all Eco Levels

Level | Entry delay (seconds) | Max latency | Average current / mA | Approximate battery life (hours)
----- | --------------------- | ----------- | -------------------- | --------------------------------
0 | N/A | N/A | 62 | 32
1 | 10 | 240 | 41 | 49
2 | 8 | 330 | 33 | 60
3 | 6 | 500 | 28 | 72
4 | 4 | 810 | 24 | 84
5 | 4 | 1360 | 22 | 93

Higher values of Eco level reduce the current consumption and increase the battery life, when the radio is idle and not receiving.
As soon as the radio receives a signal it immediately turns on all necessary hardware, and is no longer in power saving mode.

Higher values may cause the radio to not hear signals that are shorter than the overall duty cycle, so the operator needs to balance their individual need to extend the battery life with the ability to detect the signal the want to receive.

The amount of current consumption does not decrease linearly with the Eco Level value, because the radio has some core components like the CPU and voltage regulators, which always consume the same amount of current, regardless of the Eco Level.

Although the default value is 1, which results in approximately 30% less current consumption with minimal loss ability to detect a signal, values of 2, 3 work well for most people, with no noticeable loss in radio functionality.
Levels 4 and 5 may result in some degradation in the ability to detect a signal, but can be used to extend the battery life.

##### Suspend<!-- linebreak -->

This setting controls what happens when the power / volume control on the radio is turned off.
In order to maintain a realtime clock, the radio now has a "Suspend" mode which keeps the CPU running at low speed with all other radio systems turned off

If suspend mode is enabled, turning off the power / volume control puts the radio into suspend mode.
Turning on the power / volume control wakes the radio from suspend mode.

If button **SK2** is held in while the power / volume control is turned off, and with suspend mode enabled, the radio will do a full power off, and the realtime clock will not be maintained.
If suspend mode is not enabled, holding **SK2** while the power / volume control is turned off, will enter suspend mode.

*Notes:*

- Suspend mode consumes about 20mA from the battery, and will flatten the battery in around 3 or 4 days, for a brand-new battery that is fully charged.
- This mode is primarily intended for use with Satellite mode, which requires the exact time and date to be known, in order to predict satellite passes and calculate satellite Doppler corrected frequencies.

**This setting is only available on GD-77 | DM-1801 | DM-1801A.**

##### Safe Power On<!-- linebreak -->

This setting requires SK1 to be pressed when powering up the transceiver, preventing unwanted power-ups, such as when the radio is in a backpack, which can drain the battery. This parameter is also operational when suspend mode is enabled.

*Note:*

- This setting is also available on the RD-5R, even if suspend mode isn't.

**This setting is not available on the MD-9600 | RT-90.**

##### Auto Power Off<!-- linebreak -->

This setting (*APO*) enables the transceiver to switch off, if the radio is not used in the selected amount of time (30, 60, 90, 120 and 180 minutes); i.e. No keys or buttons, including PTT no keys are pressed.

One minute before the transceiver switches off, an "**Auto Pwr-Off**" message is displayed and notification beep tones are played.

*Notes:*

 - The **Auto Pwr-Off** function does not work:
   * if the transceiver is scanning.
   * if a Satellite alarm is set.
   * while in hotspot mode.
 - If **Auto Pwr-Off** function is enabled, the battery information (*percentage or voltage*) will be displayed in **bold font**.
 - If [**APO with RF**](#apo-with-rf) is enabled, the timer will also get reset if a valid signal is received.
 - Technically; the APO function uses the same low power functionality as Suspend mode, so the radio will continue to consume about 16mA when in Auto Power Off, we are currently trying to reduce this current, but because the firmware can't completely cut off power to all the radio hardware, it will never be possible to completely turn off the radio in the same way as the volume / power knob does.

##### APO with RF<!-- linebreak -->

If [**Auto Pwr-Off**](#auto-power-off) is enabled, the *APO* timer will also be reset when receiving a valid signal.

##### Sat (Satellite follow mode)<!-- linebreak -->

This setting is used to control whether in satellite mode, on the Polar or Live screens, whether the radio automatically changes to the next available satellite after the current satellite has passed over and gone below the horizon.

Default is **Manual**, and the currently selected satellite does not change. "Auto" automatically switches to the next available satellite.

##### GPS<!-- linebreak -->

This setting is only available on radios which have a GPS receiver, this includes the TYT MD-9600 | Retevis RT-90 and TYT MD-UV380 | Retevis RT-3S when they have the optional GPS receiver fitted, or when people have modified the radio to add an internal or external GPS

Because the GPS receiver consumes over 50mA constantly when in use, the GPS receiver is not powered by default.

Options are:

  - **Off**: turn off GPS module power (except on the TYT MD-9600 | Retevis RT-90 for technical reasons),
  - **On**: turn on GPS module power,
  - **NMEA**: the GPS module sends all NMEA data to the USB serial port of the radio.

**WARNING: Setting the GPS to output NMEA data will prevent the CPS communicating with the radio, and the GPS setting should be set to "Off" or "On", when using the CPS.**


<div style="page-break-after: always; break-after: page;"></div>

#### Radio Options

This menu controls various settings specific to the radio / RF functionality

##### Band Limits<!-- linebreak -->

This setting controls the frequency band ranges inside which the radio can transmit.

Options are:

- ***OFF***: where transmission is **not limited** to band ranges.
- ***ON***: where the **band limits for the USA** are applied (**this is the Default setting**):
  - 144MHz - 148MHz,
  - 222MHz - 225MHz,
  - 420MHz - 450MHz.
- ***CPS***: where the VHF and UHF limits set **in the CPS** are used. If the CPS band limits do not contain valid values, for example the UHF frequency band range is **less than** or **intersects** with the VHF band range, the radio will use the **Default** settings (as above)

![CPS band limit window](media/cps-band-limits.png)

The CPS band limits **do not affect** the overall hardware band limits, hence it **is not possible** to extend the hardware limits by using values for the CPS band limits which extend outside the hardware limits.

The hardware band limits are:

- 127MHz - 178MHz,
- 190MHz - 282MHz, (not MD-9600 | RT-90)
- 380MHz - 564MHz.

These limits are because the *AT1846S RF* chip **will not operate reliably** outside this range, and this range is actually beyond the published specification of the AT1846S, which is technically 134MHz - 174MHz, 200MHz - 260MHz, 400MHz - 520MHz.

It should also be noted that the radio does **not** have a PA or Rx section for the 200MHz band, **so operating in this range has high spurious emissions, usually on the 1<sup>st</sup> harmonic of the frequency in use**.

##### Filter time<!-- linebreak -->

This feature works when *TimeSlot* filtering is turned **off** (**Filter: Off** in the *Quick Menu*).

It sets the duration the radio listens in to one particular *TimeSlot* before resuming listening to the other *TimeSlot* for traffic.

This prevents the radio from switching to the other *TimeSlot* in the event that there is a long pause or transmission gap in the current *TimeSlot* being heard.

When **TimeSlot** filtering is turned **on** (**Filter: TS** in *Quick Menu*), this does not have any effect.

##### Scan delay<!-- linebreak -->

During scan mode, this controls the duration that the radio tunes in to a channel before resuming scan.

This works when **Pause** is selected as the scan mode.

##### Scan dwell<!-- linebreak -->

During scan mode, this controls the duration that the receiver listens (dwells) on each frequency and listens for a signal.
The default is 30 milliseconds.
On DMR if the value is less than 60 milliseconds, the value of 60 milliseconds is used, because this is the minimum time for one complete DMR frame of 2 timeslots.

Longer values can help when scanning for weak signals or signals which fade in and out, but will reduce the number of frequencies or channels scanned per second

##### Scan mode<!-- linebreak -->

This setting controls how the receiver stops when there is a signal during scan mode.

- **Hold**: continuously tunes in to a channel when a signal is received.
- **Pause**: tunes in to that signal for a specified duration (*Scan Delay*) and then resumes scan.
- **Stop**: the scan mode will exit on the first valid received signal.

##### Scan on Boot<!-- linebreak -->

This setting controls whether the radio automatically starts scanning when it's turned on (booted up).
The default for this setting is Off.

##### *xxx* Squelch<!-- linebreak -->

- **VHF**: This setting controls the squelch level for **2m VHF** when using an analog channel or during analog mode in VFO. **Default is 45%**.
- **220**: This setting controls the squelch level for **220MHz** when using an analog channel or during analog mode in VFO. **Default is 45%**.
- **UHF**: This setting controls the squelch level for **70cm UHF** when using an analog Channel or during analog mode in VFO. **Default is 45%**.

##### PTT Latch<!-- linebreak -->

When **PTT latch** is enabled, the **PTT** switch toggles the radio to transmit or receive. In this mode the PTT does not need to be pressed continuously during an over.

*Note:*

- The PTT latch function **only works** if a timeout has been defined for the Channel or VFO, to prevent constant accidental transmission.


<div style="page-break-after: always; break-after: page;"></div>

##### Allow PC<!-- linebreak -->

Allows **Private Calls** to be received.

##### User Power<!-- linebreak -->

This setting controls the PA power level when the power setting of +W- is enabled.
The value of this setting is the internal numerical value sent to the digital to analogue converter connected to the PA drive circuit.
The default value is 4100 which is the maximum possible value. Hence, by default the +W- power setting will result in the radio transmitting the maximum power it can.
The power output is normally greater than 5W, which is the official maximum power output.

On UHF (70 cm band), using a GD-77, with a fully charged battery, the power output is usually around 5.5W to 6W.
On VHF (2m band), using a GD-77, with a fully charged battery, the power output is usually somewhere between 7W and 8W.

The purpose of this setting is to give the operator the ability to not only transmit more power than the official maximum power, for example for emergency operation.
But it also allows the radio to transmit very low power levels, if low values of PA drive are used.
A value of 0 would result in no drive to the PA at all, but there will still be RF generated by the main RF / transceiver chip in the radio.
Some signal from the RF chip is likely to leak into the antenna output of the radio, and it definitely leaks through the plastic case of the radio.
So a value of 0 does not stop the radio completely from generating RF.

This setting can also be used to configure the radio to produce low levels of power e.g. below 50mW which can be useful when only transmitting to a local hotspot.

The power level for a given user setting value, varies considerably from radio to radio and will vary depending on battery voltage and transmit frequency.
The power level will also vary depending on model of radio e.g. GD-77, DM-1801 or RD-5R etc. With the RD-5R power levels being considerably different from the GD-77 and DMR-1801 because the RF and PA hardware is completely different.

A power meter is the only way to know what power output each individual radio will produce on a specific frequency, for a specific user power setting, at a specific battery voltage.

##### DMR crc<!-- linebreak -->

This settings disables the DMR CRC checking, which could be helpful in some cases while listening some specific networks.


<div style="page-break-after: always; break-after: page;"></div>

#### Display Options

##### Brightness<!-- linebreak -->

The firmware allows the display backlight brightness to be controlled from **100%** to **0%**, in **10% steps** between *10%* and *100%*, and below *10%* the brightness is controlled in **1% steps**.

- Use the **Right** and **Left** arrow keys to adjust the brightness.

The default backlight brightness (**default 100%**).

##### Nite Bright<!-- linebreak -->

This setting is identical to [Brightness](#brightness) above, except it is used when Night theme is active (see [Auto night](#auto-night)).

##### Min Bright<!-- linebreak -->

Controls the display backlight brightness in its "*Off*" state.

The default value is **0%**, so that when the display is in its **Off** state, there will be no backlight.

##### Contrast<!-- linebreak -->

The firmware allows the display contrast to be set.

Lower values result in dark text, higher values result in darker text, but the background also starts to become dark at higher settings.

##### Mode<!-- linebreak -->

Controls the display backlight operation

- **Auto** Display backlight will turn on automatically when triggered by various events *e.g.* Rx of signal, or pressing a key or button.
- **Squelch** Display backlight remains illuminated while the FM squelch is open or there is a valid DMR signal, and also remains illuminated for the specified backlight timeout after the squelch has closed. The minimum timeout period in this mode is 5 seconds.
- **Manual** Display backlight is toggled on and off by pressing the **Black** button (**SK1**).
- **None** Display backlight will not illuminate under any condition.

##### Timeout<!-- linebreak -->

Sets the time before the display backlight is extinguished (**default No timeout**).

Setting this value to "**No**" prevents the backlight from turning off at all.

##### Screen<!-- linebreak -->

This option allows for Normal or inverse colour display.

- **Normal** is white background with black pixels on monochrome platforms, theme colours are positive on coloured platforms. 
- **Inverted** is black background with white pixels on monochrome platforms, theme colours are negative on coloured platforms

*Note:*

- This does not completely replicate the GD-77 “*Black*” display hardware version, because that radio uses a different LCD panel which physically has a black background, whereas the normal GD-77 has an LCD panel with a white background.

##### Auto night<!-- linebreak -->

This option allows the firmware to automatically change the theme between Day and Night, according to daytime.

**Please Note**: the location, date and time **has** to be defined in order to make it work. These values can be defined by hand (in the [Radio info](#radio-info) screen) or automatically using the embedded GPS on featured transceivers.

The firmware calculates the sun position and switch to the correct theme when the sunrite/sunset time has come.

- On colours platforms, you can edit the two themes, using the [Theme Options](#theme-options) or the CPS.
- On monochome platforms, the firmware toggles between non inverted screen for Day, and inverted for Night. If the [Screen](#screen) display option is set to **Inverted**, the Day/Night display invertion are reversed (**Inverted** for Day, **Normal** for Night).

The user can override the current daytime theme, pressing **SK1** + **Red**, in the Channel or VFO screens **only**.

- Once the daytime theme is override, the automatic theme switching is disabled.
- if **Auto night** is set to **Off** and an override is set, it will be restored on transceiver power-up.
- Long press on **SK1** + **Red** clears this override.

##### Order<!-- linebreak -->

Controls where the DMR Contact display data is sourced from:

- **Ct**: Digital Contacts (*in the codeplug*).
- **Db**: DMR ID database.
- **TA**: Talker Alias.

The default is **Ct/Db/TA**, which means the received DMR ID is first checked in the **Digital Contacts**, and if not found the **internal DMR ID database** is searched, and if not found and the DMR transmission includes **Talker Alias**, then Talker Alias will be used.

##### Contact<!-- linebreak -->

Controls the position on the screen where the DMR Callsign and Name etc., is displayed.

Options are:

- **1 Line**: This only uses the middle line of the display to show the callsign and name. When using **Talker Alias** which contains more characters than the 16 character width of the screen, the text will be cropped, so **you will not see the end of the TA text**.
- **2 Lines**: The Callsign is displayed on the middle line of the display, and the name and other information will be displayed on the bottom line of the display. *i.e.* the firmware automatically breaks up the "**CALLSIGN NAME**" format text at the space separating the **CALLSIGN** from the **NAME**.
- **Auto**: When the Callsign and Name will fit on the middle line of the display, only the middle line will be used (this is equivalent to the "1 Line" option.). If the caller information, *e.g.* from TA, is longer than 16 characters and won't fit on the middle line, the display will be split onto both lines and is equivalent to the "2 Lines" option.

The default is **1 Line**.

##### Battery (units)<!-- linebreak -->

Controls whether the battery is show as a percentage or as voltage.

Options are:

- **%**: Shows the battery percentage *e.g.* **0%** to **100%**.
- **V**: Shows the battery voltage *e.g.* **8.1V**.


*Note:*

- This functionality does not apply to the MD-9600 | RT-90 as it is supplied from external 12V and the display always shows the voltage

##### Info<!-- linebreak -->

This setting controls whether the radio displays additional information on the VFO of Channel screen, by making the DMR Timeslot, or the Power level text bold, or both bold.

If TS or Both setting is selected, the TS value will be shown in bold if an override is applied to the TS, from a Contact TS override.
If Pwr or Both setting is selected the power value will be shown in bold if a channel specific power override is being applied to the normal power setting.

The default setting is Off, and no overrides will be shown.

##### Volume<!-- linebreak -->

**This setting is only available on the TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84.**

This setting enables the visual volume bar graph notification when rotating the volume knob.

##### LEDs<!-- linebreak -->

This setting controls whether the green / red LED on the top of the radio illuminates.
The default setting is On, so that both the LED on the top of the radio will illuminate green on Rx and red on Tx
If this setting is set to off, the LED will not illuminate either on Rx or Tx.

##### Timezone<!-- linebreak -->

This setting allows you to set the local timezone.

Press the **Right** arrow to increase the value in steps of 1 hour.

Press the **Left** arrow to increase the value in steps of 1 hour.

If your timezone is not on a 1-hour boundary, press **SK2** and **Right** or **Left** to adjust the timezone in 15 minute increments.

##### Time (display format)<!-- linebreak -->

This setting controls whether the value of time and date that is entered and displayed is "UTC" or "Local"

When this is set to Local, it uses the value set in Radio Information Timezone to calculate the date and time for the clock date and satellite passes

If "UTC" is selected, all dates and times displayed will have UTC after the value to indicate that UTC is being used.
If "Local" is selected, dates and times do not show any text to indicate that Local time is use

##### Show dist(ance)<!-- linebreak -->

This setting enables the display of the distance to repeater (in kilometers) to the right of the Zone name, in the Channel screen.

To have it working, Channel's location has to be set (using the CPS), and the transceiver location has to be valid (Radio Info's [Location screen](#location-screen) or GPS).

If both locations aren't set or valid, **"--- km"** will be displayed instead.

<div style="page-break-after: always; break-after: page;"></div>

#### Sound Options

##### Timeout beep<!-- linebreak -->

This setting controls whether the radio emits timeout warning beeps during transmission when the timeout is about to expire and transmission will be terminated.

##### Beep volume<!-- linebreak -->

This controls the volume of the beep and other tones, and can be set from **100%** to **10%** in these increments: (**-24dB**, **-21dB**, **-18dB**, **-15dB**, **-12dB**, **-9dB**, **-6dB**, **-3dB**, **0dB**, **3dB**, **6dB**).

##### DMR Beep<!-- linebreak -->

This setting controls the beeps which are played at the **start** or **end**, or **both** start and end of DMR transmissions.

The beep at the start of transmissions is used to confirm connection to a repeater, because it is only played when the radio enters the main transmission phase to a repeater, and not when its '**waking**' the repeater.

These beeps are only played through the radio's speaker, they are not transmitted via the DMR audio signal.

Options are:

- **None**
- **Start**
- **Stop**
- **Both**

##### RX Beep<!-- linebreak -->

This controls the emission of specific beeps when receiving a signal (FM and DMR), based on the presence of an RF carrier and/or a talker (DMR only).

Options are:

- **None**
- **Carrier**
- **Talker** (see [*Talker*](#talker) option below)
- **Both**

*Note:* 

- If **Talker** is selected, in FM the beeps tones will be the identical as DMR's Talker ones instead of regular **Carrier** ones.

##### Talker<!-- linebreak -->

This controls the **RX Beep** *Talker* option. It could limit the beep to the talker's transmission ending when **End only** is selected, or enable beeps on talker's transmission beginning/ending when selecting **Both**.

Options are:

- **End only**
- **Both**

##### DMR mic<!-- linebreak -->

This controls the audio gain of the DMR microphone input system, relative to the default value.

This only adjusts the gain on DMR, and does not affect the FM mic gain.

Settings are in **3dB steps**, with **0dB being the normal default setting**, which is the same as the official firmware.

##### FM mic<!-- linebreak -->

This controls the audio gain of the FM microphone input system, **relative to the default value**.

- Positive values result in more gain than default,
- Negative values result in less gain than default.

The units of this control in the baseband IC (*AT1846S*) **are not known**.

##### VOX threshold<!-- linebreak -->

Threshold value which controls the mic level which **triggers** the radio to transmit when VOX is enabled.

##### VOX Tail<!-- linebreak -->

Controls the length of time **after** the operator stops speaking, before the transmission is ended.

##### Prompt<!-- linebreak -->

This setting controls the **audible feedback** to button and key presses etc. and has the following options:

- **Silent**: The radio does not provide any audio feedback to button
- **Beep**: The radio emits a beep when keys or buttons are pressed. There are 2 different pitches of beep.

    When navigating through *Channels* or *Talkgroups* or *menu items*, when the first item in the list is reached the **higher pitch** beep is emitted.

    Also, when switching between *Timeslots*, the **higher pitch** beep is emitted on **TS1**.

    When **switching between FM and DMR** mode the **higher pitch** beep is emitted when the mode is **DMR**.

    When changing power, the **higher pitch** beep is emitted when the **lowest power level is selected**.

- **No Keys**: Identical as **Beep** (see above), except it doesn't emit any beep on button and key presses.
- In addition to the beep, the firmware also supports voice prompts **if a voice prompt file is loaded via the CPS**.

There are 3 levels of voice prompt:

  - "**Voice**",
  - "**Voice L2**" and
  - "**Voice L3**", in the latter two cases the L indicates the "Level"

  The voice level is used to control whether the voice prompt is played immediately, or whether the operator needs to press button SK1 to play the which describes the last change made to the radio.

  For example. On **Voice** mode, which is **level 1**, the things which are voiced immediately voiced are:

  - Number key, and # key buttons being pressed.
  - Changes to squelch level.
  - Menu options are announced as you arrow through the menu system, as well as the "*Quick*" menus accessed via the Orange button on the top of the radio.
  - Option values are announced as you change menu settings.

  Voice **level 2** has almost identical operation to Voice **level 1**, except that if a key or button is pressed while a prompt is already being played, **there will be a slight reduction in the verbosity of the next response**.

  Voice **level 3**, all items voice **immediately**, including:
  - Channel names are announced as you arrow through channels in channel mode;
  - Talkgroup names are announced as you arrow through them in DMR mode;

  Voice prompts can be **re-announced** by pressing the **SK1** button.

  For example, if the last voice prompt was the *Talkgroup name*, then pressing **SK1** will play the **Talkgroup name again**.

  Pressing **SK1** whilst a voice prompt is playing, **terminates the voice prompt playback**.

##### DMR Rx AGC<!-- linebreak -->

This setting controls the DMR audio leveling function.


When this function is enabled, the firmware monitors the peak amplitude of the DMR Rx audio, and adjusts the audio output gain so that the audio amplitude from the speaker remains more constantly.
By default this is disabled. Set to Off.

Setting this to 0dB (gain boost) enables this function.
Increasing the AGC value, increases the additional audio gain which is applied. Hence increasing the value will increase the overall volume of the audio.
Operators in high noise environments can increase this value to make the radio speaker level louder that has previously been possible, however if the AGC value is increased too much, it will result in clipping of the audio signal and result in distortion when receiving from some stations.

Like most AGC systems, the audio leveling uses a sample window period and also a level control low pass filter, so that normal changes to voice audio amplitude are not leveled out.
Hence it takes approximately 1 second for the AGC to adjust to each new DMR signal which is received.
However the AGC control level for each DMR station which is received, is stored as part of the Last Heard data, so that if the same station is heard again, the last known AGC value for that station is applied immediately, hence the audio level is changed immediately and does not take 1 second to adjust to the level of that station.

It should be noted that this system is not perfect and some variation in audio level will be observed.
During testing, it was noted that signals received via gateways from other networks or people using phone Apps etc; often have much higher audio levels, and sometimes that output gain control hardware in the radio is not able to attenuate the signal enough to ensure the audio is at the same level as DMR signals from DMR networks.

##### Click suppr<!-- linebreak -->

**This setting is only available on the MD-9600 | RT-90 and controls the Click Suppression function.**

Some models of MD-9600 | RT-90 emit a loud click when the audio amplifier is turned on. To reduce this, the Click Suppression function can be enabled, however a quiet click can still be heard.

To completely remove the click requires a hardware modification to the radio by the user.

#### Language<!-- linebreak -->

This screen allows the language of the on-screen texts to be selected.

*Notes:*

- This does not change the language of the Voice Prompts, because the voice prompts are not part of the main firmware file and must be loaded separately using the OpenGD77 CPS.
- Not all languages are actively maintained by the original native translator, so the translations of some languages are not perfect.

If you noticed a problem with a language translation, please post to the https://www.opengd77.com forum, providing a better translation.

#### Calibration screen<!-- linebreak -->

**This screen currently only applies to the TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84.**

##### Cal Freq<!-- linebreak -->

This selects the current calibration point. This is the frequency that the radio will transmit on and the Power Adjust setting will change.  There are 5 calibration points for VHF and 8 calibration points for UHF. The firmware interpolates between these points to calculate the calibration required for other frequencies.
Hence to calibrate the power for the 2M band, the 136.0MHz, 145.5MHz and 155.0MHz calibration points must all be adjusted. This is because 144-148 MHz spans multiple points. 

##### Cal Power<!-- linebreak -->

For each calibration point, there are 4 power levels which need to be calibrated. 250mW, 1W, 2W and 4W

##### Power Adjust<!-- linebreak -->

This value controls the amount of PA drive. This is a 8 bit number, and hence has a range from 0 to 255, where 0 is no PA drive and 255 is maximum PA drive.

##### Freq Adjust<!-- linebreak --> 

This value adjusts the master frequency reference oscillators. This is a 8 bit number, and hence has a range from 0 to 255. To lower the frequency, decrease this value, to increase the frequency , increase this value.

*Note:*

- There are separate reference oscillators for VHF and UHF. Therefore the frequency should be adjusted twice. Once with a VHF calibration point and once with a UHF one. The calibration point used for each band is unimportant and the frequency calibration only needs to be done once on each band.  

##### Factory Cal<!-- linebreak -->

This value allows the calibration to be restored to the factory defaults. This will normally show "No"
To restore factory defaults, set this to "Yes" and press the Green button.
After the factory calibration has been applied, this setting returns to "No"

##### Calibration Procedure<!-- linebreak -->

1. To calibrate the Tx power of the radio you will need a power meter and a dummy load.
2. Connect the radio to the power meter.
3. Connect the dummy load to the antenna connection of the power meter.
4. Select the desired Tx calibration point.
5. Select the power level (e.g. 250mW)
6. Press the PTT and adjust the Power Adjust value, until the power meter shows 250mW.
7. Repeat steps 5 and 6 for all other power levels
8. Repeat steps 4 to 7 for all other calibration points.

When power calibration has been completed, pressing **Green** exits from the calibration screen, retaining the current settings in RAM only.
To permanently save the settings press **SK2** + **Green** 

However, to temporarily test the power e.g. by transmitting using the VFO, pressing **Green** on its own is OK.  You can return back to the calibration screen, after testing using the VFO and the values you adjusted will be used.

#### Theme Options<!-- linebreak -->

**This screen currently only applies to the TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84.**

##### Theme Chooser<!-- linebreak -->

In this screen, you can select the Day or Night theme (see Display [Auto night](#auto-night) option).

Press **Green** to enter the theme options screen (see below).

##### Theme Options<!-- linebreak -->

![theme options screen](media/theme-menu.png)

In this screen, you can adjust theme items colours.

- Press **Hash** key to edit the selected item colour (see [*available theme items*](#here-is-the-detailed-list-of-the-theme-items)),
- Press the **Green** key to validate the new theme colour, **all changes are temporary**,
- Press **SK2** + **Green** key, to make the changes permanent,
- Press **SK1** + **Green** key to get back to defaut theme (Black & White), temporary (just reboot to restore the latest saved theme),
- Press **SK1** + **SK2** + **Green** key, the default theme (Black & White) will be restored **permanently** (erasing the previously stored theme),
- Press **Red** key to cancel all the changes.


<div style="page-break-after: always; break-after: page;"></div>

##### Colour Picker<!-- linebreak -->

Item's colour edition.

![colour picker](media/colour-picker.png)

In the colour picker screen, you can change the *Red*, *Green* and *Blue* colour channel values (using **Left** and **Right** buttons (*or rotary control on platforms like the RT-3S*)).

If you press the **SK2** button while changing the value, the step is increased by a factor of 3.

  The default increment/decrement step are:

   - 8 for *Red* and *Blue* (with a max value of 248),
   - 4 for *Green* (with a max value of 252).

*Note:*

- all these step and max values are related to the colour format (RGB 565).

- Press **Green** key to validate the new colour. **Red** key cancels the change.


<div style="page-break-after: always; break-after: page;"></div>

##### Here is the detailed list of the theme items<!-- linebreak -->

![theme items part 1](media/theme-items-1.svg)<!-- linebreak -->

![theme items part 2](media/theme-items-2.svg)

<div style="page-break-after: always; break-after: page;"></div>

#### APRS Options

##### Beaconing Mode<!-- linebreak -->

This setting let you select the beaconing mode.

Modes are:

- **Off** No beaconing at all
- **Manual** Using **SK1** + **2** key, while in the Channel or VFO screen, transmits an APRS beacon.
- **PTT** A beacon will be send when releasing the **PTT** key, honoring the **Interval** timer (e.g, *Initial* set to *1min*, *Decay* set to *Off*: the interval between two beacons can't be less than one minute).
- **Auto** A beacon is automatically send at timed intervals (see **Interval** setting below).
- **Smart** Use the SmartBeaconing&trade; algorithm for automatic beaconing (see below).

*Note*: When in the Channel or VFO screen, the APRS beaconing could be temporary toggled **On** or **Off**, using the **SK1** + **1** key. 


##### Beaconing Location<!-- linebreak -->

This setting permits to choose the location source used to report your position.

Available options are:

- **Channel** Uses APRS configuration (see [FM APRS location transmission](#fm-aprs-location-transmission)) or the position entered in the Radio Info's [Location screen](#location-screen).
- **GPS** Uses the embedded GPS to report your position/speed/direction.


##### Beaconing Initial Interval<!-- linebreak -->

This defines the initial interval for automatic beacon transmissions.

This value is used in when **PTT** or **Auto** is selected.


##### Beaconing Decay Algorithm<!-- linebreak -->

This setting controls the Decay algorithm which continuouly extends the beacon transmission interval in the case that there is no change in the position information. (see [Interval](#beaconing-initial-interval) above).

When your position does not change, the decay algorythm doubles the interval beaconing time, with a maximum of 32 times the Interval value.

Example:

- Interval is set to 1 minute.
- The beaconing interval will be (if the position doesn't change meanwhile):  
  1 minute, 2 minutes, 4 minutes, 8 minutes, 16 minutes, 32 minutes, 32 minutes, 32 minutes...


##### Beaconing Compression<!-- linebreak -->

This enables the APRS compression (position/speed/direction). This reduces transmissions time.


##### SmartBeaconing&trade;<!-- linebreak -->

SmartBeaconing&trade; is a beaconing algorithm invented by Tony Arnerich KD7TA and Steve Bragg KA9MVA.

This optimizes beacon transmission based on direction and speed.

The firmware also embed some presets, which you could also tweak to match your needs.

Presets are selectable using the keypad key:

| Key | Preset |
| --- | --- |
| **0** | Default values |
| **1** | Car |
| **2** | e-Bike |
| **3** | Bike |
| **4** | Walking |
| **5** | Sailing |
| **6** | APRSdroid |

The algorithm is tunable using the following settings (see next sections):

- [Slow Rate](#slow-rate)
- [Fast Rate](#fast-rate)
- [Low Speed](#low-speed)
- [High Speed](#high-speed)
- [Turn Angle](#turn-angle)
- [Turn Slope](#turn-slope)
- [Turn Time](#turn-time)


##### Slow Rate<!-- linebreak -->

How often beacons will be send when your speed is equal or below the **Low Speed** value.

Value in minutes: from **1** up to **100**, default is **30**.

- If you press the **SK2** button while changing the value, the step is increased by a factor of 10.


##### Fast Rate<!-- linebreak -->

How often beacons will be send when your speed is equal or above the **High Speed** value.

Value in seconds: from **10** up to **180**, default is **120**.

- If you press the **SK2** button while changing the value, the step is increased by a factor of 10.


##### Low Speed<!-- linebreak -->

When your speed is equal or lower than this, beacons are transmitted at the time interval defined in **Low Rate** time interval.

Value in km/h: from **2** up to **30**, default is **5**.

- If you press the **SK2** button while changing the value, the step is increased by a factor of 4.


##### High Speed<!-- linebreak -->

At this speed or above, beacons will be transmitted at the **Fast Rate** time interval.

Value in km/h: from **2** up to **90**, default is **70**.

- If you press the **SK2** button while changing the value, the step is increased by a factor of 10.


##### Turn Angle<!-- linebreak -->

The minimum angle by which you must change course before it will trigger a beacon.

Value in degrees: from **5** up to **90**, default is **28**.

- If you press the **SK2** button while changing the value, the step is increased by a factor of 10.


##### Turn Slope<!-- linebreak -->

This number, when divided by your current speed (in mp/h) will be added to the Turn Angle value in order to increase the turn threshold at lower speeds.

The calculated value will never exceed 120&deg;.

Value in 10&deg;/speed: from **1** up to **255**, default is **26**.

- If you press the **SK2** button while changing the value, the step is increased by a factor of 10.


##### Turn Time<!-- linebreak -->

The minimum time interval between beacons when you are continuously changing direction.

Value in seconds: from **5** up to **180**, default is **60**.

- If you press the **SK2** button while changing the value, the step is increased by a factor of 10.


<div style="page-break-after: always; break-after: page;"></div>

### Channel Details

![channel details screen](media/channel-details.png)

#### Channel name<!-- linebreak -->

Displays the channel name, and also allows the name to be changed.

A flashing underline is shown at the current text insertion position, which will initially be after the last text character of the name.

Pressing the appropriate button on the numerical keypad, enters numbers and letters. e.g. The "2" button, initially enters 2, but immediately pressing "2" again enters the letter "A"

Pressing **SK2** + **Left**, deletes a character.

#### RX<!-- linebreak -->

Rx frequency.

Enter the frequency via the keypad.

#### TX<!-- linebreak -->

Tx frequency.

Enter the frequency via the keypad (or use [**Repeater Shifts**](#repeater-shifts)).

##### Repeater Shifts<!-- linebreak -->
Most of the standard repeater shifts are supported by the firmware.

When the Tx or Rx frequency has the focus, **Left** or **Right** buttons (*or rotary control on platforms like the RT-3S*) will apply a shift on the Rx frequency to set the Tx one.

The supported values are:

 - 0.0*MHz*, &#177;600*kHz*, &#177;1.0*MHz*, &#177;1.5*MHz*, &#177;1.6*MHz*, &#177;2.0*MHz*, &#177;4.6*MHz*, &#177;5.0*MHz*, &#177;7.0*MHz*, &#177;7.6*MHz*, &#177;9.0*MHz* and &#177;9.4*MHz*.

![repeater shift popup](media/repeater_shift.png)

#### Mode<!-- linebreak -->

*FM* or *DMR*.

#### DMR ID<!-- linebreak -->

If the channel mode is DMR, a channel specific DMR ID number can be entered via the keypad.

#### Color Code<!-- linebreak -->

Sets the *Color Code* when the VFO / Channel is set to **DMR**.

#### Timeslot<!-- linebreak -->

Selects DMR *Timeslot* 1 or 2 when the VFO / Channel is set to **DMR**.

#### TG Lst<!-- linebreak -->

Selects which *TG list* is assigned to the current channel (**DMR only**).<!-- linebreak -->

*Note:* 

- Only *TG Lst* **OR** *Contact* could be selected at once.

#### Contact&nbsp;<!-- linebreak -->

Selects which *Contact* is assigned to the current channel (**DMR only**).<!-- linebreak -->

*Note:* 

- Only *Contact* **OR** *TG Lst* could be selected at once.

#### Rx CSS (CTCSS or DCS)<!-- linebreak -->

Sets the *receive CTCSS tone or DCS code* when the VFO / Channel is set to **FM**.

For both Tx and Rx CTCSS / DCS:

- **Long press**, **Right** or **Left** arrows, skips forward, or back by 5 entries in the list of possible CTCSS / DCS settings.
- Pressing **SK2** + **Right** or **SK2** + **Left** skips to the end or beginning of the current CTCSS / DCS items.

#### Tx CSS (CTCSS or DCS)<!-- linebreak -->

Sets the *transmit CTCSS tone or DCS code* when the VFO / Channel is set to **FM**.

#### BW<!-- linebreak -->

Sets the *Rx and Tx bandwidth* in **FM** mode to either **25Khz** or **12.5Khz**.

#### Step<!-- linebreak -->

Selects the VFO / Channel frequency step size.

#### TOT<!-- linebreak -->

Sets the time-out timer to **OFF** or **ON**.

#### Rx Only<!-- linebreak -->

Set the channel to receive only is this value is **ON**.
When the channel is set to receive only, pressing the PTT results in the "ERROR Rx Only" message and the radio will not transmit.

#### Zone Skip<!-- linebreak -->

Set to *skip the Channel* when scanning within the *zone*.

#### All Skip<!-- linebreak -->

Set to *skip the channel* when scanning within the **All Channels** zone.

#### VOX<!-- linebreak -->

Controls whether VOX (Voice Operated Switch) is enabled or disabled.

#### Ch Power<!-- linebreak -->

Controls the custom / individual power assigned to the channel.

See also the section in about controlling power.

**By default**, all channels will use the **Master** power setting, and this option allows a **custom** power setting to be set on a channel, or for the channel set to use the **Master** power setting.

#### Squelch (Channel)<!-- linebreak -->

Controls the custom / individual squelch assigned to the channel.

See also the section in about controlling power.

**By default**, all channels will use the **Master** squelch setting. This is the squelch value defined in the Options squelch setting for the band of the channel.
A **custom** squelch setting can be applied to the channel by pressing the right and left arrow keys. Custom squelch settings are in 5% steps.

#### Beep (Channel)<!-- linebreak -->

Controls whether beeps are played on the channel.
By default beeps are enabled on all channels, but beeps can be disabled on individual channels by setting this option to No.

#### Eco (Channel)<!-- linebreak -->

Controls whether Eco modes function on this channel.
By default Eco modes are enabled on all channels, but Eco mode can be disabled on individual by setting this option to No.

#### TA Tx TS*x*<!-- linebreak -->

Enables **transmission** of *Talker Alias* data on the specified Timeslot (TS1/TS2).

Options are:

- **Off**: no Talker Alias transmission.
- **APRS**: the position, if defined in "**Radio Info**" screen (or by the GPS module, on featured platforms) is used for this transmission.
- **Text**: the text of **Line1** and **Line2** from the "**Boot Item**" CPS screen is used for this transmission, with no space between the **Line1** and **Line2** data.
- **Both**: send both informations listed above, alternatively.

*Notes:*

- Talker Alias reception is always operational. Do not enable this feature because you are not receiving TA data, as it does not control TA Rx.
- Use of this feature **will cause problems on Motorola based repeaters and networks**, and should only be used for simplex and possibly on *Brandmeister* and other networks which correctly support Talker Alias. -->


#### APRS (channel)<!-- linebreak -->

Sets the FM APRS Tx configation to be used on this VFO / Channel

The default setting is None


#### Accepting and saving the changes to the channel<!-- linebreak -->

- Pressing the **Green** menu key confirms the changes.
- Pressing **SK2** + **Green** saves the settings to the codeplug, or in the case of the VFO the changes are saved to the non-volatile settings.
- Pressing the **Red** menu key closes the menu without making any changes to the channel.


<div style="page-break-after: always; break-after: page;"></div>

### Satellite Screen

This screen predicts when Amateur Radio satellites will pass overhead the current location, for the next 24 hours using the location, date and time entered by the operator.
It also automatically corrects for Doppler shift on both the Tx and Rx frequencies, as well as displays the azimuth and elevation of the satellite in a variety of ways, including numerical and polar plots.

Before this screen can be used, the operator **MUST** enter their location, as well as the current time / date into the Radio Info screen.
Also, the satellite orbital data Keps' **MUST** be uploaded using the CPS.

If the operator has not entered the date / time or location, they will be prompted to do this.

For example, after power cycling radios, that do not have real time clocks in them, the date and time will be cleared, and they need to be re-entered.
At the time of writing only the MD-9600/RT-90, UV380/RT-3S and DM-1701 have real time clock hardware.

Uploading the latest Keps' from the CPS also sets the date and time, so in practice it's often easier to upload the Keps' than to set the date / time manually

When using the satellite functionality the operator does **not** need to set the satellite frequency or CTCSS, as these values are uploaded from the CPS as part of the Kep's data and date / time upload
To change the satellite frequencies or upload different satellites, the satellites.txt installed as part of the CPS can be modified.

For satellites like SO-50, which have an "Arming" CTCSS tone. Press SK1 during transmission to transmit the "Arm" CTCSS tone.
For more details on Amateur Radio satellite operation, see the AMSAT website   https://www.amsat.org 


The first screen displayed is the master predictions list. This lists the prediction of all passes for all satellites in the next 24 hours, displayed chronologically.

![location](media/satellite-main-predictions-list.png)


Because of the number of calculations that need to be performed, the predictions take a few seconds to be calculated. While this is happening a progress bar is shown.

Once the list appears, it shows the satellite name as well as the time that the satellite will appear above the horizon (known as Acquisition of Satellite - AOS), and the maximum elevation in degrees
If a satellite is currently above the horizon, this is shown by a black bar on the right side of the screen next to that satellite / pass.

![location](media/satellite-main-predictions-list-AOS.png)

Use the **Down** / **Up** arrows to scroll down / up through the list.


*Notes:*

- Some satellites, e.g. SO-86 are on an equatorial orbit and only pass over equatorial locations, hence passes for that satellite will not appear in the predictions list for locations outside this geographic area.
- For current satellite operation status information see the AMSAT status page  https://www.amsat.org/status/


Pressing **Green** to select a specific satellite / pass displays the predicted **Polar view** for that satellite / pass.


#### Polar view<!-- linebreak -->

![location](media/satellite-polar-before-AOS.png)

The polar view graphic shows the path of the satellite shown as a plan view from vertically above the location of the radio, with the outside circle being the horizon, and the two inner circles being 30 deg and 60 deg and the centre being directly overhead the location.
When the satellite is currently below the horizon, a large dot is show where the satellite will appear on the horizon.
If the satellite is above the horizon, the dot shows the current position of the satellite.

When the satellite is below the horizon, the time to the next pass is shown in the top left of the screen in either -HH:MM:SS or -MM:SS or -SS s depending on how long it is until the pass
When the satellite is below the horizon, the maximum elevation is shown in the bottom left of the screen.

When the satellite is above the horizon, the current Azimuth is shown the top left corner of the screen, the current elevation is shown in the bottom left of the screen, and the satellite position is shown on the polar plot.

![location](media/satellite-polar-mid-pass.png)

Further, in the same pass, the display changes, every second, to show the movement of the satellite as well as changes in azimuth and elevation

![location](media/satellite-polar-mid-pass-2.png)


The current RSSI signal strength is shown at all times as a vertical bar, so that operators can adjust their antennas for maximum signal.

On this screen, the squelch and power can be adjusted using the same keys as on the Channel and VFO screens.

Press **Down** to enter the individual satellite predictions screen, or **Up** to enter the satellite live data screen


#### Satellite individual predictions screen<!-- linebreak -->

![location](media/satellite-individual-passes-1.png)


This screen allows the predictions for individual satellites to be viewed, including the time and maximum elevation of the pass and the duration of the pass.

Press **Right** / **Left** to step through the pass predictions for the currently selected satellite

![location](media/satellite-individual-passes-2.png)


Press **Down** to enter the satellite live data screen or **Up** to enter the Polar view.


#### Satellite live data screen<!-- linebreak -->

This screen shows the current Azimuth and Elevation of the selected satellite, regardless of which pass has been selected.
It also shows the current Transmit and Receive, the power level, and the battery voltage.

Negative elevation values indicate that the current satellite is below the horizon

The firmware and CPS support 3 different Tx/Rx frequencies for each satellite, these are 

1. FM Voice Tx/Rx frequency
2. APRS Tx/Rx frequency
3. Beacon Rx only frequency.

The frequency type is shown on the right side of the screen.
If the satellite does not have an APRS or beacon frequency, then no frequency values are displayed, and as beacons by their nature are Rx only the Tx frequency is not displayed

Attempting to transmit on a frequency where Tx is not supported, e.g. the beacon frequency, the firmware will not allow transmission and will pay the warning beep sound instead

To select the Voice, APRS or Beacon fequency, press the keys 1, 2 or 3 respectively.

*Note:* 

- Keys 1, 2 and 3 currently only operate on this screen and not the Polar or other satellite screens.

![location](media/satellite-live-before-AOS.png)

The screen updates once a second to continuously update.

![location](media/satellite-live-mid-pass.png)

![location](media/satellite-live-mid-pass-2.png)

On the Polar, Live and Individual satellite predictions screens. Press SK2 + **Up** / **Down** to change to a different satellite.

*Note:*

- If a satellite has no passes over the current location, the radio will display "Pass: None" or "Empty List" depending on the screen currently selected.
e.g. IO-86 only passes over equatorial locations.

#### Squelch and Power settings<!-- linebreak -->

In all Satellite screens, **except** the [Satellite individual predictions](#satellite-individual-predictions-screen) one, it's possible to adjust the Squelch and output Power settings using the following keys:

- Squelch:
  - on **GD-77 | DM-1801 | DM-1801A | RD-5R | TYT MD-9600 | Retevis RT-90 | Baofeng DM-1701 | Retevis RT-84**, use the **Left** and **Right** keys.
  - on **TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84**, use the rotary knob.
- Power:
  - on **GD-77 | DM-1801 | DM-1801A | RD-5R | TYT MD-9600 | Retevis RT-90 | Baofeng DM-1701 | Retevis RT-84**, use the **SK2** + **Left** and **SK2** + **Right** keys.
  - on **TYT MD-UV380 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84**, use **SK2** + rotary knob.
  - **except on the TYT MD-UV380 | Retevis RT-3S** for technical reasons, you can access the **+W-** power setting using **SK2** + **Long press** **Right** keys. 

#### Satellite alarm<!-- linebreak -->

To be alerted about a specific satellite pass:

 - Press **SK2** + **Green** on any of the satellite screens before 1 minute prior to that pass, the radio will go in suspend mode to save the battery, **except on MD-9600 | RT-90**.
 - 1 minute before the satellite is predicted to appear above the horizon, the radio will resume from suspend mode then emits an alarm beep.
 - Press any keypad key to silence the alarm.

To manually resume from suspend mode, press:
 - **Orange** button on GD-77 | GD-77S | DM-1801 | DM-1801A | RD-5R (check [variations between different supported radios](#variations-between-different-supported-radios) section for DM-1701 | RT-84) 
 - **SK2** + **PTT** buttons on MD-UV380 | RT-3S.

To cancel the alarm once it has started:
 - Press **Green** key, or turn the radio on / off.

If the satellite pass alarm (1 minute long) is not canceled (using the **Green** key), the radio will go back in suspend mode, still in the optic of battery saving.


#### CPS Integration<!-- linebreak -->

The CPS has an extra feature added to download the Kep's data and upload this to the radio, as well as setting the date / time of the radio.
In the Extras -> OpenGD77 support screen of the CPS. Connect the USB cable to the radio, make sure the radio is turned on, and press the "Install satellite Keps" button.
The CPS defaults to downloading the Keps from a specific web URL, however if the operator prefers to use a different source of Kep's data, they can change the URL.

The satellites which are imported and uploaded to the radio are defined in the file satellites.txt which is installed with the CPS into its installation directory.
This file is a standard format CSV file, and contains the satellite catalog number, as well as the display name in the radio, and the Tx, Rx frequencies and Tx CTCSS as well as the "Arming" CTCSS for satellites which use an "Arming" tone.
The operator can edit this file to add or remove satellites as required.
The maximum number of satellites which can be loaded into the radio is 25, but currently there are 8 AMSAT satellites in this data

| **Cat#** | **Name** | **Rx1** | **Tx1** | **CTCSS**| **Arm CTCSS** | **Rx2** | **Tx2** | **Rx3** | **Tx3** | **APRS Config** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 22825U | AO27 | 436.795 | 145.850 | 0 | 0 | 0 | 0 | 0 | 0 ||
| 43017U | AO91 | 145.960 | 435.250 | 67 | 0 | 0 |0 | 0 | 0 ||
| 40908U | CAS3H | 437.200 | 144.350 | 0 | 0 | 0 | 0 | 437.200 | 0 ||
| 40931U | IO86 | 435.880 | 145.880 | 88.5 | 0 | 0 | 0 | 0 | 0 ||
| 43678U | PO101 | 145.900 | 437.500 | 141.3 | 0 | 145.900 | 437.500 | 0 | 0 ||
| 25544U | ISS | 437.800 | 145.990 | 67 | 0 | 145.825 | 145.825 | 0 | 0 | ARISS 0WIDE2 1 |
| 27607U | SO50 | 436.795 | 145.850 | 67 | 74.4 | 0 | 0 | 0 | 0 | |
| 54684U | FO118 | 435.600 | 145.925 | 67 | 0 | 435.650 | 0 | 435.570 | 0 ||
| 51069U | TEVEL2 | 436.400 | 145.970 | 0 | 0 | 0 | 0 | 436.400 | 0 ||
| 0988U | TEVEL3 | 436.400 | 145.970 | 0 | 0 | 0 | 0 | 436.400 | 0 ||
| 51063U | TEVEL4 | 436.400 | 145.970 | 0 | 0 | 0 | 0 | 436.400 | 0 ||
| 50998U | TEVEL5 | 436.400 | 145.970 | 0 | 0 | 0 | 0 | 436.400 | 0 ||
| 50999U | TEVEL6 | 436.400 | 145.970 | 0 | 0 | 0 | 0 | 436.400 | 0 ||
| 51062U | TEVEL7 | 436.400 | 145.970 | 0 | 0 | 0 | 0 | 436.400 | 0 ||


#### Technical notes<!-- linebreak -->

The satellite position and prediction calculations are generated in real time by the firmware in the radio, and the currently selected satellite data is updated once per second.

The predictions are usually accurate to around +/- 5 seconds of AOS time, LOS time and duration, compared with other satellite prediction software including AMSAT's online prediction page and other PC applications like GPredict
Prediction programs like GPredict usually don't show exactly same values for start, or end, to the online AMSAT predictions either.

Predictions will not be completely accurate unless the satellite Kep's data is updated frequently. If practical the keps should be uploaded on a daily basis, though normally the satellites don't move too far from their predicted path for several days, or even a week.

The prediction calculation is a custom implementation, written for the OpenGD77, using the methodology from the original AMSAT prediction calculation called PLAN13 written in the 1983.
See https://www.amsat.org/amsat/articles/g3ruh/111.html


<div style="page-break-after: always; break-after: page;"></div>

### GPS Screen

The GPS screen is currently only available on the TYT MD-UV380 | MD-UV390 | Retevis RT-3S | Baofeng DM-1701 | Retevis RT-84 and TYT MD-9600 | Retevis RT-90 for radios which have GPS fitted, or in the case of the MD-9600 where users have modified the radio to attach and internal or external GPS module

Because the GPS receiver consumes over 50mA constantly when in use, the GPS receiver is not powered by default in the MD-UV380 | RT-3S | DM-1701 | RT-84 firmware.
GPS power state could be changed in this screen using **Green** + **SK2** and **Red** + **SK2** (available value are the same than in **General Options**).

On the MD-9600, it's possible to enable the GPS power (but not to enable the NMEA output) by long pressing **Green** key (**ENT** on the front panel and **A/B** on the mic).

To use the GPS receiver in the radio, you must first enable the GPS in the [**General Options**](#gps) menu.
If the radio is not fitted with GPS, or the GPS does not appear to function, this option will show the value "None".
If the radio is fitted with a GPS, the value of this option will initially display "Off"
To use the GPS, change this value to "On", or "NMEA". Setting the GPS to NMEA will enable the GPS module and send all NMEA data from the GPS module to the USB serial port of the radio.

*Notes:*

- Setting the GPS to output NMEA data will prevent the CPS communicating with the radio, and the GPS setting should be set to "Off" or "On", when using the CPS.
- The GPS receive in both the MD-UV380 and MD-9600 is not very sensitive, and can take a long time to acquire the position, and the GPS in these radios does not work indoors.

Initially after turning on the GPS, the GPS screen will show the text "Acquiring".  On the UV380 signal strength bars for any satellites which the GPS is receiving will also be displayed.
On the MD-9600 version, there is not enough room on the first GPS screen to show the signal strength bars, so they are shown on a second page to the GPS screen, which is accessed by pressing the **Down** arrow button


![MD-UV380 GPS Acquiring](media/MD-UV380-GPS_Acquiring.png)

![MD-9600 GPS Acquiring](media/MD9600-GPS_Acquiring.png)

Both the MD-UV380 and MD-9600 versions also have a page in the GPS screen, which shows the polar positions of any detected GPS satellites, however this screen is not functional until the GPS position is known.

Once the GPS position has been acquired, the position will be displayed, including Latitude, Longitude, Locator and position accuracy.

![MD-UV390 GPS Acquired](media/MD-UV380-GPS_Acquired.png)

![MD-9600 GPS Acquired](media/MD9600-GPS_Acquired.png)

![MD-9600 GPS RSSI](media/MD9600-GPS_RSSI.png)

Polar view

![MD-UV390 GPS Polar view](media/MD-UV380-GPS_Polar.png)

![MD-9600 GPS Polar view](media/MD9600-GPS_Polar.png)


<div style="page-break-after: always; break-after: page;"></div>

More position information and direction

![MD-9600 Position view](media/MD9600-GPS_Pos_2.png)

![MD-UV380 Direction view](media/MD-UV380-GPS_Direction.png)

![MD-9600 Direction view](media/MD9600-GPS_Direction.png)

*Note:*

- The heading information (compass arrow, degrees and cardinals) are only displayed when the speed is greater than zero.


<div style="page-break-after: always; break-after: page;"></div>

**The center of the heading compass is displaying the Fix quality:**

| **Symbol** | **Fix Quality** |
| --- | --- |
| ![No Fix](media/GPS_No_Fix.png) | No Fix |
| ![Low Q Fix](media/GPS_Low_Q_Fix.png) | Low |
| ![2D Fix](media/GPS_2D_Fix.png) | 2D |
| ![3D Fix](media/GPS_3D_Fix.png) | 3D |


**The GPS automatically updates the Real Time clock in the radio, and the position is used for DMR APRS transmissions.**

On the UV380 | RT-3S | DM-1701 RT-84 the GPS satellite RSSI bar graphs are colour coded. By default, Blue is for USA GPS Satellites and Red is for other satellite systems.


<div style="page-break-after: always; break-after: page;"></div>

## Making and receiving DMR Private Calls

### To make a Private Call

In DMR mode, either in the VFO or the Channel screen:

- Press the **#** key twice to enter the *Private Call DMR ID*
- The top of the screen will now show “**PC entry**”
- Enter the station’s DMR ID *e.g.* **5053238**
- Press the **Green** menu key to confirm, or the **Red** menu key to exit.

*Notes:*

- If you make a mistake when entering the number, press the **Left** arrow key to erase the digits one by one.
- If the PC ID you entered is in the DMR ID database you had previously uploaded to the radio, the station Callsign and name will now be displayed on the screen.
- If the ID is not in the DMR ID database, the text, “**ID:**“ followed by the number, will be displayed

**The radio is now in Private call mode.**

To return to normal Talkgroup operation, there are 3 methods:

1. Press **SK2** + **Red** menu key.
2. Press the **Left** or **Right** arrow key which will load the next TG in the TG list assigned to the VFO or the Channel.
3. Press the **Hash** (**#**) key, then enter a TG number and press the **Green** menu key.


*Note:*

- When in *Private Call* mode, changing between VFO mode and Channel mode or vice versa, via the **Red** menu key will not change back to *TalkGroup* mode.

### To Receive a Private Call<!-- linebreak -->

On receipt of a *Private Call*, the radio will display this screen:

![accept screen](media/accept-call.png)

With the callers *Callsign* and *Name* (or ID) displayed.

To accept the call, and configure the radio to return the Private call back to the calling station:

- Press the **Green** menu key, for YES.
- Otherwise, either press the **Red** menu key for No, or ignore the prompt and continue using the radio as normal.

If you accept the Private Call, the radio will be switched into **Private Call mode**, ready for transmission.

The caller's ID or Name is shown *e.g.*:

![private call screen](media/private-call.png)

Once the Private Call is complete, you can return to the *Talkgroup* you were on prior to accepting the Private Call, by pressing **SK2** + **Red** menu key. (or by any of the methods described in the section on making a **Private Call**).


<div style="page-break-after: always; break-after: page;"></div>

## Hotspot mode

**IMPORTANT INFORMATION**

**Hotspot mode is not supported on the Baofeng RD-5R | DM-5R because the hardware does not support reliable USB communications while the radio is transmitting**

- The USB connection between the radio and the host system *e.g.* Pi-Star **needs to be protected from RF injection**, otherwise the USB connection will **occasionally be reset** when the radio is transmitting, which will cause the hotspot to **stop working**.
- **Do not use the antenna on top of the radio** when in hotspot mode, this usually causes RF injection problems which **can't** be resolved by screening or ferrite chokes.
- Connect the radio to an **external antenna**.
- Use **ferrite** RFI protection on the USB cable.
- When using a Raspberry Pi as the host system, use a **metal enclosure** for the Raspberry Pi.

The firmware can operate as a DMR (**voice only**) hotspot when connected via its USB programming cable to a Raspberry Pi running Pi-Star, or *any other device* that is running MMDVMHost.

*Note:*

- Hotspot mode may be compatible with software like **BlueDV**, but your mileage may vary.

First, connect the radio to a Raspberry Pi via its programming cable.

![a hotspot hardware](media/hotspot-connections.jpg)<!-- { width=600 } -->

Hotspot mode works with the Raspberry Pi Zero, but an adaptor cable is needed to convert from the micro USB port on the RPi Zero to the full size USB plug on the radio's programming cable.


<div style="page-break-after: always; break-after: page;"></div>

In the Pi-Star Configuration screen, select “**OpenGD77 DMR hotspot (USB)**” as the modem type.

![Pi-Star configuration page](media/pistar-configuration.png)

If your version of Pi-Star does not contain the OpenGD77 DMR Hotspot as an option, please **update** your version of Pi-Star.

Assuming the modem type has been set properly in Pi-Star, the display will change on the radio to show it is in **Hotspot Mode**, and will show the *Color Code*, *Receive frequency* and approximate *TX power* in mW.

![hotspot screen](media/hotspot-mode.jpg)

If the radio still fails to enter hotspot mode, check your USB connections.

*Note:*

- By default, Pi-Star configures the “modem” to have a power setting of “100” in the Expert -> MMDVMHost settings.

This is 100% of the maximum power of the modem, and in the case of the radio the maximum power output is **5W**, but the radio is not designed to operate as a hotspot, where it may be continuously transmitting.

The maximum power setting that the radio can support for continuous transmission will vary depending on the operating environment, including the ambient temperature and antenna SWR, etc.

It is the responsibility of the user to set an appropriate power level that will not overheat and damage the PA.

In Hotspot mode, if Pi-Star (MMDVMHost) sends a power setting of 100%, the assumption is that Pi-Star has not been correctly configured for the OpenGD77 and this value is disregarded.

Instead, the firmware will use the current (Channel or VFO) power setting, which will default to 1W.

If the power setting in the Pi-Star MMDVMHost Expert settings is any other value *e.g.* **50%**, the hotspot will use that power setting closest to the chosen value.
So **50%** of *5W* is **2.5W**, and the closest power setting to this is *2W*.

**Power matching tables:**

- **5W Handhelds**

  | **Power** | **Pi-Star RFLevel** |
  | --- | --- |
  | 50mW | 1 |
  | 250mW | 5 |
  | 500mW | 10 |
  | 750mW | 15 |
  | 1W | 20 |
  | 2W | 40 |
  | 4W | 80 |
  | 5W | 99 |
  | +W- | N/A |

- **MD-9600**

  | **Power** | **Pi-Star RFLevel** |
  | --- | --- |
  | 100mW | 1 |
  | 250mW | 5 |
  | 500mW | 10 |
  | 750mW | 15 |
  | 1W | 20 |
  | 5W | 40 |
  | 10W | 60 |
  | 25W | 80 |
  | 40W | 99 |
  | +W- | N/A |


The receive frequency specified by Pi-Star will be displayed at the bottom of the screen.

*Note:*

- Offsets **should not be applied** to the TX or RX frequencies in Pi-Star, because the radio should not need any offsets, and any offset will be reflected in the frequency displayed on the radio, because Pi-Star actually sends the master frequency +/- the offset to the hotspot.

When the radio receives an RF DMR signal, the green LED on the top of the radio will illuminate as normal, and the name and callsign are displayed if the DMR ID database contains that ID. If the ID is not in the DMR ID database, the ID number will be shown.

![hotspot RX screen](media/hotspot-rx.jpg)

When Pi-Star receives traffic from the Internet and sends it to the hotspot for transmission, the hotspot displays the Callsign and name or the DMR ID, and the TX frequency is shown.

The LED on the top of the radio also turns red to indicate the radio is transmitting.


<div style="page-break-after: always; break-after: page;"></div>

## Resetting the Settings

The radio can also be set to the default settings by holding the **SK2** key (**P3** on the MD-9600 | RT-90) while turning on the radio.

Additionally, holding the:

- **SK2** button as well as the **Up** and **Down** arrow keys on the GD-77 | DM-1801 | DM-1801A | RD-5R,
- **SK2** button as well as the **Down** arrow key on the MD-UV380 | RT-3S | DM-1701 | RT-84 | MD-2017 | RT-82,
- **P3** button as well as the **Down** front panel arrow key on the MD-9600 | RT-90,

resets **any** custom boot melody, custom boot image and themes on colours platforms, that has been uploaded using the OpenGD77 CPS.

On the GD-77S, which does not have a keypad, holding **SK2** and **Orange** resets **any** custom boot melody.


<div style="page-break-after: always; break-after: page;"></div>

## GD-77S operation

To use the firmware with the GD-77S you **must** load voice prompt files using the OpenGD77 CPS. If you do not load voice files the radio will not announce anything, **and it will be virtually unusable**.

See the section relating to voice prompts and how to install them.

The GD-77S has a **16 positions** rotary switch on the top of the radio, next to the volume control.

This control is used to select the Channel in the current Zone.

*Note:*

- Although the OpenGD77 CPS and codeplug format allows up to 80 channels per Zone, the GD-77S can **only access the first 16 channels** in each Zone, so codeplugs designed for the GD-77 containing more than 16 channels will **need** to be modified so that each zone only contains a maximum of 16 channels.

The GD-77S has 2 buttons on the side of the radio below the **PTT** button. A **Black** button known as **SK1** and a **Function** button known as **SK2**. It also has an **Orange** coloured button at the top, next to the channel selector switch.

The firmware uses the concepts of different **Control modes**.

In each mode, buttons **SK1** and **SK2** perform a different function, the operator cycles through the **Control modes** by pressing the **Orange** button.

The **Control modes**, and the function of buttons **SK1** and **SK2** in each mode is as follows:

### GD77S Channel / TG mode

This mode is announced as "**Channel mode**".
In this mode, button **SK1** and **SK2** are used to cycle through the *Talkgroups* / *Contacts* assigned to the current channels

### GD77S Scan mode

This mode is similar to the Channel scan mode in the normal firmware.

Pressing **SK1** toggles scanning to **start** or **stop**, in the same way that holding the **Up** and **Down** arrows controls the Zone scan function in the normal firmware.

### GD77S Timeslot mode

In this mode, pressing either button **SK1** or **SK2** toggles from *Timeslot 1* to *Timeslot 2*.

### GD77S Color Code mode

In this mode, pressing **SK1** increases the *Color Code* number, and pressing **SK2** decreases the *Color Code* number.

### GD77S DMR Filter mode

In this mode, pressing **SK1** increases the *DMR filter level* and pressing **SK2** reduces the *filter level*.

See information in the normal firmware, in the VFO or Channel screen quick menu, for details for DMR filter levels.

### GD77S Zone mode

In this mode pressing **SK1** or **SK2** cycles through the *Zones*, pressing **SK1** selects the *next Zone* and pressing **SK2** selects the *previous Zone*.

Zone selection wraps around, so pressing **SK2** on the first Zone, selects the *last Zone*, and pressing **SK1** on the last Zone selects the 8first zone*.

### GD77S Power mode

In this mode, pressing **SK1** increases the power *by one step*, and pressing **SK2** decreases the power *by one step*.

See details of available power step levels in the normal firmware.

*Note:*

- Like in the normal firmware, the power output will only be accurate if the operator **has calibrated** the power of the radio, as the factory power level calibration is likely to be highly inaccurate.


<div style="page-break-after: always; break-after: page;"></div>

## MD-9600 and RT-90 specific

The TYT MD-9600 | Retevis RT-90 uses the following keys and buttons

![MD-9600 | RT-90 overview](media/MD9600Controls.jpg)<!-- { width=600 } -->


<div style="page-break-after: always; break-after: page;"></div>

**Front panel:**

| **Key** | **Function** |
| --- | --- |
| P1 | **SK2** |
| P2 | **SK1** |
| P2 | (*NO FUNCTION*) |
| P4 | **Star** (*) |


Rotary control changes channel or frequency, and menu settings.

On the VFO and Channel screens, the **Up** and **Down** arrow map to the **Right** and **Left** button functionality on the handheld radios. e.g. On FM, increase and decrease squelch.
In menu screens, the **Up** and **Down** buttons move up or down within the menu's.

On the Channel screen, **Long press** of the **Up** arrow button, starts scanning.

During scanning pressing the **Down** arrow button, or **C** button on the mic, reverses the direction of scan.

During scanning the **B** button on the mic, or the front panel **Up** arrow, marks the channel as a nuisance channel. This is the same functionality as the **Right** button on the handheld radios.

VFO scanning can not be operated from the front panel buttons.

**On the mic keypad:**

| **Key** | **Function** |
| --- | --- |
| A/B | **Green** |
| A | **Red** |
| B | **Right** |
| C | **Left** |

**Long press** of **D** key toggles **SK2** latch, so SK2 functions can be controlled from the mic.

When entering or directly transmitting DTMF on FM, the following key mappings are used to send or enter the A, B, C and D characters:

| **Key(s)** | **DTMF** |
| --- | --- |
| **Up** | A |
| **SK1** + **Up** | B |
| **Down** | C |
| **SK1** + **Down** | D |


<div style="page-break-after: always; break-after: page;"></div>

## CPS software

*Note:*

- You **cannot** use the standard Radioddity CPS, or Baofeng CPS, to write to a radio flashed with the firmware.
If you wish to use the Radioddity CPS the radio will **need to run the official Radioddity firmware**. Once the codeplug has been written to the radio with your ID and callsign, you can then flash the firmware to the radio, and it will then read and operate with the code plug written to it with the standard firmware and CPS software.

Please download the latest OpenGD77 CPS from the location given in [section 1.1](#download-links-and-other-resources))


Please see the next section for information specific to the OpenGD77 CPS. The information in the rest of this section is applicable to both the standard Radioddity CPS and the OpenGD77 CPS.

### Overview

The firmware simplifies the concept of TalkGroups, for maximum convenience for radio amateurs. Unlike most commercial DMR radios it is not necessary to create multiple channels to use the same frequency with many different transmit TalkGroups. Changing is as simple as scrolling **Left** and **Right** across your TalkGroup list or entering an *ad hoc* TalkGroup by pressing the **hash** key.

In DMR mode when using either the VFO or the Zones and Channels, you can use the **Left** / **Right** arrow keys to scroll through and select any of the TalkGroups in the TG list assigned to the current channel, or to VFO A.

When programming the radio using the CPS, first add all the **TalkGroups** that you think you may wish to use into the *Digital Contacts* list.

![CPS TG contact lists](media/cps-tg-contacts.png)

Next create one or more “**TG Lists**” and populate each with the sets of the *Talkgroups* that you will want to use with different channels. You can have the same *Talkgroups* in **many** *TG Lists*.

![TG list window](media/cps-TGlists.png)

Now set up the **Channels**. Enter the frequencies, slot and color code as normal for a DMR channel.

Next select the **TG List** that you wish to use for the channel.

The firmware can use the *TG list* to filter the incoming DMR signal, or it can operate in “*Digital Monitor Mode*” (aka promiscuous mode) all the time. This can be set in the radio quick menu setting for **Filter** and **DMR filter**.

![channel TG list selection](media/cps-channel-tglist.png)<!-- { width=600 } -->

*Note:*

- You must use the *TG list* to define the TG’s you want to use with each Channel. Hence, you must have at least **1 TG list** and it must contain at least **1 Digital Contact** which is a *TalkGroup*.

Finally, save your codeplug to your computer before writing the code plug to the radio using either the standard Radioddity CPS to program the radio before flashing it to OpenGD77, or, if you are using the special OpenGD77 compatible version of the CPS, (as detailed in the next section) you can write the codeplug directly to an already flashed OpenGD77 radio.

#### New Driver Installation<!-- linebreak -->

The CPS installer now also installs the comm port driver, however the comm port driver can be installed manually by downloading the files from the location given in [section 1.1](#download-links-and-other-resources))


To install the driver, download and unzip the zip file, and run the .bat file

Once the driver is installed, the Windows device manager should show the “**OpenGD77**” in the “*ports*” section of the Windows device manager

![Device manager window](media/device-manager-ports.png)<!-- { width=280 } -->

#### OpenGD77 Menu<!-- linebreak -->

In the CPS, there is a new menu item under the Extras menu, for OpenGD77 Support, which opens this window.

![OpenGD77 support window](media/cps-opengd77-support.png)<!-- { width=480 } -->

From here you can **backup** the internal **64k EEPROM** and the **1 megabyte Flash** chip, as well as Reading and Writing the codeplug.

The calibration data stored in the Flash chip (At address *0x8f000*) can be backed up and restored without backing up the whole of the Flash.

*Note:*

- If you restore the Flash you will also **overwrite the calibration data** as it’s stored in the 1Mb Flash chip.

You can also use this window to grab a screenshot from the radio's current display. Screenshots are saved in PNG format.


<div style="page-break-after: always; break-after: page;"></div>

#### Backup Before You Do Anything Else<!-- linebreak -->

Before writing a codeplug to the radio the first time, you should **backup both the EEPROM and Flash** chip, and save the files in a **safe place**, in case something goes wrong in the future and you need to restore the data.

![menu entry to access the OpenGD77 support window](media/Backup-01.png)

Backup the **EEPROM**, **Flash memory**, **Calibration data**, **MCU ROM** and the **Codeplug**.

![buttons that create various backups](media/Backup-02.png)<!-- { width=550 } -->

#### Reading and Writing Your Codeplug<!-- linebreak -->

To read the codeplug, press the “Read codeplug” button, wait for all 3 data sections to download, and then close the OpenGD77 Support window. To write a codeplug press the “Write codeplug” button.

#### Writing DMR IDs -- the User Database<!-- linebreak -->

The firmware supports **extended DMR ID information**, with up to 50 characters, for Callsign, Name, City, etc.

Please change the Number of characters menu to the desired DMR callsign and name length.

Then, you can add in DMR IDs into the database by **selecting an ID prefix**. You can continue adding DMR IDs based on your commonly heard prefixes until you fill up the allocation.

![DMR IDs downloader window](media/cps-dmr-ids.png)<!-- { width=550 } -->

*Note:*

- Because the memory size used for the DMR ID is **limited**, you can store more DMR IDs if you assign fewer characters per ID. Depending on actual information, the firmware can store approximately **13,800** to **69,600** IDs in its user database.

As the firmware supports **Talker Alias**, you might find this sufficient. The firmware will display Callsign and Name data retrieved from the DMR stream, for user IDs not stored in your radio's User Database.


<div style="page-break-after: always; break-after: page;"></div>

#### Boot tune<!-- linebreak -->

The tones are in pitch, delay pairs. So **38,6** means play **tone 38** (*932Hz F#*) for **6 time periods**.

##### Boot Tune in Morse code<!-- linebreak -->

You can create your callsign in Morse code when turning on the radio. ITU Morse standards have the following ratios:

- **38,6**: dash
- **0,2**: internal pause
- **38,2**: dot
- **0,6**: interchar pause
- **0,7**: interword pause (**unused in a Callsign**)

Or perhaps more usefully:

- **Dah**: 38,6,0,2,
- **Dit**: 38,2,0,2,

  and change the terminating "**2**" to a **6** between letters. (*No comma on the very end*).

  So **KI4** (*for example*) would become:

  - **38,6,0,2, 38,2,0,2, 38,6,0,6,**
  - **38,2,0,2, 38,2,0,6,**
  - **38,2,0,2, 38,2,0,2, 38,2,0,2, 38,2,0,2, 38,6,0,6**
- Remove the spaces and carriage returns once you've got it all worked out and paste into the Boot Tune section under Extras/OpenGD77 support

##### Melodies and Notes<!-- linebreak -->

For reference, the tone values in OpenGD77 are:

| **Value** | **Note** | **Freq** | **(info)** | | | **(Hz)** | | | | | | | | | |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **1**  | A  | 110  | (A2) | 13 | A  | 220 | | 25 | A  | 440 | | 37 | A  | 880 |   |
| **2**  | A# | 116.5 | | 14 | A# | 223   | | 26 | A# | 466 | | 38 | A# | 932.3 | |
| **3**  | B  | 123.5 | | 15 | B  | 247   | | 27 | B  | 494 | | 39 | B  | 987.8 | |
| **4**  | C  | 130.8 | (C3) | 16 | C  | 261 | (C4 mid c)| 28 | C  | 587.3| (C5) | 40 | C  | 1046.5 | (C6) |
| **5**  | C# | 138.5 | | 17 | C# | 277   | | 29 | C# | 554.3 | | 41 | C# | 1108.7 | |
| **6**  | D  | 146.8 | | 18 | D  | 294   | | 30 | D  | 587.3 | | 42 | D  | 1174.7 | |
| **7**  | D# | 155.5 | | 19 | D# | 311   | | 31 | D# | 622.3 | | 43 | D# | 1244.5 | |
| **8**  | E  | 164.8 | | 20 | E  | 329.6 | | 32 | E  | 659.3 | | 44 | E  | 1318.5 | |
| **9**  | F  | 174.6 | | 21 | F  | 349   | | 33 | F  | 698.5 | | 45 | F  | 1397 | |
| **10** | F# | 185   | | 22 | F# | 370   | | 34 | F# | 740 | | | | | |
| **11** | G  | 196   | | 23 | G  | 392   | | 35 | G  | 784 | | | | | |
| **12** | G# | 207.6 | | 24 | G# | 415.3 | | 36 | G# | 830.6 | | | | | |

#### Boot Image<!-- linebreak -->

The Boot image needs to be **128 wide x 64 pixels high**. It needs to be in **1-bit PNG format**. (*An indexed image format that is not supported by some modern paint programs*).
