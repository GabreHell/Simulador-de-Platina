# Simulador-de-Platina
Um dashboard interativo em tempo real para calcular e projetar o tempo necessário para atingir os 100% de conclusão (Platina) em videojogos.
Este projeto é uma visualização de dados interativa desenhada para testar diferentes cenários e planear o tempo necessário para completar videojogos a 100%.

Tecnologias: Desenvolvido com HTML, JavaScript e Tailwind CSS para garantir um design moderno e responsivo.

Interatividade: Utiliza deslizadores dinâmicos para ajustar a duração do jogo base e a disponibilidade de horas semanais.

Cálculo em Tempo Real: Inclui alternadores para adicionar DLCs ou o multiplicador de tempo da Platina, atualizando imediatamente as horas totais, as semanas necessárias e a data de conclusão projetada.

## Como executar

Baixe o repositório e abra [simulador_de_platina.html](simulador_de_platina.html) no navegador. Se preferir usar Git:

```sh
git clone https://github.com/GabreHell/Simulador-de-Platina.git
cd Simulador-de-Platina
```

Não é necessário instalar dependências ou compilar o projeto. A apresentação visual utiliza Tailwind CSS via CDN e a fonte Inter via Google Fonts, portanto requer internet para carregar esses recursos.

## Como usar

1. Ajuste a duração do jogo base, entre 10 e 200 horas.
2. Informe sua disponibilidade semanal, entre 1 e 40 horas.
3. Ative **Modo Platinar / 100%** e **Incluir DLCs/Expansões**, se desejar.
4. Confira as horas totais, as semanas estimadas e a data projetada.

## Regras de cálculo

- Platina: multiplica o tempo base por 1,5.
- DLCs: acrescenta 15 horas após o multiplicador.
- Semanas: divide as horas totais pela disponibilidade semanal.
- Data: soma o equivalente em dias à data atual do dispositivo.

Por exemplo, 50 horas de jogo base, com platina e DLCs, resultam em 90 horas. Com 10 horas semanais, a estimativa é de 9 semanas.

Esses valores são hipóteses fixas de simulação, não dados reais de cada jogo. A tela arredonda as horas para um inteiro e as semanas para uma casa decimal; a projeção da data usa o cálculo sem esse arredondamento. As escolhas não são salvas ao recarregar a página.
