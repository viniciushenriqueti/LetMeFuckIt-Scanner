# LetMeFuckIt Scanner AutoPWNED 
Scanner and Exploit Magento 

O Scanner explora a vulnerabilidade **SQLi Vulnerability (1.9.1.0 CE)** do Magento.

A vulnerabilidade foi corrigida no **Patch SUPEE-5344**, entretanto, há muitas lojas que não aplicaram o patch de segurança. 

O **LetMeFuckIt** foi escrito em Python e utiliza as seguintes bibliotecas:

*pygoogle, argparse, urllib2, requests, base64*

## Uso: ##
    letmefuckit.py --dork <dork> --pages <number> --user <user> --pwd <pass>

## Exemplo: ##
    letmefuckit.py --dork "inurl:customer/account/login/ site:com.br" --pages 4 --user adm --pwd pass

## Opções ##

--dork <dork>
--user <user>
--pwd <password>
--pages <number>
--help 

## Dorks Recomendadas##

"inurl:/customer/account/login site:com.br"
"inurl:/checkout/onepage/ site:com.br"

 
## Informações ##

Através da dork inserida, é feita uma varredura no Google, as urls são salvas no arquivo urls.txt, que posteriormente são automaticamente testadas.

Os usuários fornecidos na execução são adicionados automaticamente como administradores nos sites vulneráveis.

## Screenshots ##

![](http://i.imgur.com/6lJtrv1.jpg)

![](http://i.imgur.com/KuK3S95.png)

![](http://i.imgur.com/DSVEoSz.jpg)

## Créditos ##

Exploit: Magento Shoplift exploit (SUPEE-5344) by Manish Kishan Tanwar AKA error1046 in 25/08/2015
 
LetMeFuckIt Scanner AutoPwned por OntheFrontLine in 27/09/2015