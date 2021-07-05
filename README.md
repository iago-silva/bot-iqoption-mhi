# Ferramentas utilizadas

- Windows 10
- Python 3.8.3

(lembrar de baixar o [projeto da api](https://github.com/Lu-Yi-Hsun/iqoptionapi) e rodar o comando `python setup.py install` para instalar as dependências necessárias para o seu python)

# Modo de usar

- Abra o arquivo "mhi.py" e altere as constantes EMAIL e SENHA com as suas credenciais da corretora
- Abra o CMD
- Navegue até a pasta do projeto
- Rode o seguinte comando `python mhi.py`
- O programa vai pedir 3 informações
    - O par no qual vai operar (ex: EURUSD)
    - Seu Stop Gain (O Stop Loss é o HIT)
    - Quantidade de ciclos do MHI para atingir a meta

# Como funciona

O programa vai dividir o seu Stop Gain pela quantidade de ciclos desejada. Por exemplo:

Digamos que o programa está rodando na seguinte situação:

| Informação | Valor |
| --- | --- |
| Stop Gain | 10 |
| Ciclos | 2 |
| Payout atual do par | 90% |

O programa vai fazer 2 ciclos do MHI com entrada base de 5,56. Dessa forma, com base no payout atual, se você ganhar os 2 ciclos, sairá com 10 de lucro
