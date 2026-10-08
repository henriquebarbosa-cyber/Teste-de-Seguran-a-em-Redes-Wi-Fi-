# Análise de Segurança de Rede Wi-Fi com Ferramentas Nativas do Windows

## Introdução

Este trabalho tem como objetivo analisar informações relacionadas à segurança de uma rede Wi-Fi por meio de ferramentas disponíveis no sistema operacional Windows. Para a atividade, foi utilizada uma rede de laboratório denominada **casadavovo**, permitindo observar informações como SSID, BSSID, tipo de autenticação, criptografia, intensidade do sinal e configurações do perfil de rede.

## Desenvolvimento

Para realizar a atividade prática, foi utilizado um adaptador Wi-Fi USB conectado ao computador. Inicialmente, foi executado o comando:

```bash
netsh wlan show networks mode=bssid
```

Esse comando permitiu identificar a rede de laboratório casadavovo e obter informações relacionadas ao seu funcionamento.Resultados obtidos:SSID: casadavovo  
Tipo de rede: Infraestrutura  
Autenticação: WPA2-Personal  
Criptografia: CCMP  
BSSID: a6:fb:c1:d8:8c:0b  
Sinal: 100%  
Rádio: 802.11ac  
Canal: 13

Detecção da rede casadavovoEm seguida, foi utilizado o comando:

```
netsh wlan show profile name="casadavovo"
```

permitindo consultar as configurações do perfil Wi-Fi salvo no computador.Informações do perfil Wi-Fi casadavovoPosteriormente, foi executado o comando:

```
netsh wlan show profile name="casadavovo" key=clear
```

conforme solicitado na atividade, para verificar as configurações de segurança do perfil. 
O resultado indicou que havia uma chave de segurança configurada, porém o conteúdo da chave não foi exibido no ambiente utilizado.Verificação das configurações de segurança do perfil

#Conclusão
A realização da atividade permitiu compreender, na prática, como é possível obter informações sobre uma rede Wi-Fi utilizando ferramentas nativas do Windows. Foi possível identificar o SSID, BSSID, tipo de autenticação, criptografia, canal e intensidade do sinal da rede utilizada no laboratório, além de analisar as configurações do perfil Wi-Fi salvo.A atividade também demonstrou a importância da utilização de mecanismos de segurança adequados em redes sem fio. O uso de protocolos de segurança atuais, senhas fortes, atualizações e outras medidas de proteção contribui para reduzir os riscos de acessos não autorizados e aumentar a segurança da rede.

#Evidencia
![Detecção da rede casadavovo](images/deteccao-da-rede-casadavovo.PNG)

![Informações do perfil Wi-Fi casadavovo](images/informacoes-do-perfil-wifi-casadavovo.PNG)

![Verificação das configurações de segurança do perfil](images/verificacao-configuracoes-seguranca-perfil.PNG)






