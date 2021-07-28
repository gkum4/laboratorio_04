# Laboratório 04

- Disciplina do curso de Engenharia Eletrônica da UTFPR (Universidade Tecnológica Federal do Paraná)
- Sistemas Microcontrolados (ELF52-S11)

## Observações Exercício 20.5

A partir do endereço base da porta J (GPIO_PORTJ_BASE) e do endereço de GPIO_RIS foi possível identificar qual botão foi pressionado dentro da rotina de interrupção (GPIOJ_Handler), podendo atráves de condicional realizar a adição da contagem binária caso o botão for o SW1 e a subtração caso o botão for o SW2. Foi necessário habilitar o uso do botão SW2 na sub-rotina Button_int_conf, alterando a atribuição do valor de R2 para #00000011b.