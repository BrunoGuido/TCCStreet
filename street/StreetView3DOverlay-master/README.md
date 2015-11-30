# Introdução StreetView3DOverlay

- Os modelos 3D não se encaixavam direito no mapa (google maps) de acordo com a localização (latitude,longitude) que o mesmo deveria estar localizado.
- Agora a versão nova possui modelos 3D , na anterior não possuia, possuia apenas textos..
A principal funcionalidade do aplicativo é descrever uma cena de um crime em tempo real, remodelando toda a cena para um ambiente virtual 3D, no caso usamos  aplicação Web, e a API do google Maps, para utilizarmos o serviço do Street View.
Nesse caso o servidor do google é chamado sempre que precisamos utilizar uma coordenada do serviço do street view, assim por parâmetros especificamos o serviço que estamos querendo utilizar do mesmo.
Um dos problemas da aplicação é se o serviço que estamos solicitando, fazendo a chamada estiver fora do ar, ou até mesmo não tivermos acesso a Internet, a aplicação não irá funcionar já que o serviço está sendo solicitando a todo momento que é realizada uma chamada ao servidor.

Futuramente queremos otimizar a aplicação, com o uso de óculus de imersão, assim incluiremos na aplicação técnicas de realidade virtual, outra melhoria seria o fato do usuário poder interagir diretamente com o ambiente, com o uso de sensores de movimento, podendo movimentar por exemplos os objetos da cena, assim a chamada ao servidor é realizada a todo momento que o ambiente for modificado, o serviço é solicitado a todo momento para que o ambiente do street view seja atualizado a todo momento que o mesmo sofra alterações.


## Nota de Release a Ser Publicado

•	Descrever uma cena de um crime, reconstruída em ambiente Virtual 3D
•	Imergir ao ambiente virtual com utilização de dispositivos estereoscópicos
•	Interagir com o ambiente virtual com utilização de dispositivos de sensores de movimento

##Problemas Conhecidos e Limitações

Limitação 

Para  utilizar o serviço do google maps, no caso de sua aplicação, é necessário gerar uma chave (key) para sua máquina que será o servidor, essa chave é gratuita, porém seu site ou aplicação fica limitado a 25 mil  carregamentos (LOAD) de mapas por dia, durante 90 dias, caso seu site ou sua aplicação ultrapasse esse limite, deve obrigatoriamente pagar para uso de além desse limite, comprando a licença (key) Premium.

Caso seu site ultrapasse esse limite, o google irá contatar o responsável com informações sobre as opções de pagamento,  Nesse momento, vai ser especificado um prazo de compra, até esse prazo o site vai continuar a funcionar como esperado , sem qualquer alteração ao modo como mapas aparecer.

Uma vez que o prazo já passou, se você tiver habilitado nem faturamento nem comprado uma API do Google Maps para licença de trabalho por este prazo, os mapas em seu site continuará a funcionar, mas apenas para os primeiros 25.000 mapa cargas a cada dia. Além deste número, a API do Google Maps irá parar de funcionar.


##Datas Importantes

Segue abaixo as datas importante do desenvolvimento:

22/11/15	Início do planejamento

05/01/16	Início do desenvolvimento
17/07/16	Entrega para teste
22/10/16	Fim do teste
27/11/16	Liberação para produção


##	COMPATIBILIDADE

Navegadores	Browser:
•	Mozila Firefox
•	Chrome
•	Opera
Sistema operacional	Windows 8.1
Linguagem de programação	Javascript + HTML
Framework WEB	                 Java,Javascript
IDE 	  JetBrains  WebStorm 10.0.4
Design pattern	
Servidor Web	            Google

##Procedimento e Alteração de Configuração do Ambiente

Deve Ser instalado o Banco de Dados SQL Server 2014, para que os dados sobre as cenas do crime sejam armazenados no mesmo, um arquivo de banco de dados com todas as cenas do crime é utilizado no projeto.
Instalado o IDE JetBrains WebStorm 10.0.4
Instalar um Navegador (Browser) Google Chrome
Instalar versão Java Framework Web
Instalar Javascript Framework


##Atividades Realizadas no Período

Cod  - Título - Tarefa
1   - Implementação Realidade Virtual  - Nessa liberação foi realizado a versão para realidade virtual com utilização do dispositivo óculus Rift.

Situação - Concluído 

===========================================================

2 - Sistema de Visualização do Mapa 
Tarefa - Possibilitar o usuário entre visualização panorâmica ou perspectiva, sendo Mapa 2D, ou mapa 3D, também se o mesmo deseja a opção de realidade virtual da cena.

Situação - Em Andamento 

Obs = Provavelmente irá ser migrado o sistema para a IDE do Unity, pelas dificuldade do serviço para Web/Navegador

=================================

3 Interação com o Ambiente Virtual
Possibilitar o usuário interagir com os elementos que compôem a cena do crime, os objetos tridimensionais


Planejamento 

Aguardando a entrega do dispositivo de sensor







## Credits
The ferris wheel 3D model has been downloaded from <http://www.archibaseplanet.com/download/33b26753.html>, transformed to obj with <http://www.greentoken.de/onlineconv/> and then to the three.js format with <https://github.com/mrdoob/three.js/blob/master/utils/converters/obj/convert_obj_three.py>.

## three.js
<http://threejs.org/>
The MIT License
Copyright (c) 2010-2013 three.js authors

### jQuery
Copyright 2005, 2013 jQuery Foundation, Inc. and other contributors
Released under the MIT license
<http://jquery.org/license>

### jQuery mouse wheel
Copyright (c) 2013 Brandon Aaron <http://brandon.aaron.sh>
Licensed under the MIT License
Version: 3.1.6