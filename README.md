# Como Desativar o Zoom pelo mouse no League of Legends

![League](/assets/img/lol.png)
*Créditos: [Epic games](https://store.epicgames.com/en-US/p/league-of-legends)*

Olá player de Lolzinho.

Este guia explica como configurar o **RollerButtonSpeed** para desativar o zoom com o scroll do mouse no League of
Legends. Existem duas formas de realizar a configuração: editando o arquivo `input.ini` ou o arquivo `PersistedSettings.json`.

---

## Localize o Diretório de Instalação do League of Legends

Por padrão, o League of Legends é instalado em:
```script
C:\Riot Games\League of Legends\
```

Se você alterou o diretório de instalação, ajuste o caminho conforme necessário.

---

## Método 1: Editando o arquivo `input.ini`

1. Navegue até o diretório:

```script
C:\Riot Games\League of Legends\Config
```

2. Abra o arquivo `input.ini` em um editor de texto, como o **Bloco de Notas**.

3. Adicione ou edite as seguintes linhas:
```script
[MouseSettings]
RollerButtonSpeed=0
```

![Input.ini](/assets/img/01-exemplo-input-ini.png)  

*Exemplo no arquivo input.ini*

4. Salve o arquivo e feche o editor de texto.

---

## Método 2: Editando o arquivo `PersistedSettings.json`

1. Navegue até o diretório:
```script
C:\Riot Games\League of Legends\Config
```

2. Abra o arquivo `PersistedSettings.json` em um editor de texto.

3. Adicione ou edite o seguinte bloco de código no arquivo:
```script
{
   "name": "MouseSettings",
   "settings": [
       {
           "name": "RollerButtonSpeed",
           "value": "0"
       }
   ]
} 
```

![Input.ini](/assets/img/02-exemplo-persisted-settings.png)
*Exemplo no arquivo PersistedSettings.json*

**Nota:** Certifique-se de manter a estrutura JSON válida. Não remova ou edite outras seções, a menos que saiba o que
está fazendo.

4. Salve o arquivo e feche o editor de texto.

---

## Dicas Finais

- Após realizar qualquer uma das configurações, reinicie o cliente do League of Legends para que as alterações sejam
  aplicadas.
- Caso algo dê errado, você pode excluir os arquivos `input.ini` e/ou `PersistedSettings.json`, pois o cliente recriará
  versões padrão desses arquivos ao iniciar.

---

## Referência

Para mais informações sobre como desativar o zoom pelo scroll do mouse, consulte a discussão
na [Reddit](https://www.reddit.com/r/leagueoflegends/comments/tvib4a/disable_zooming_inout_with_mouse_scroll_wheel/?rdt=56391).