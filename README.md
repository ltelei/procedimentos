# procedimentos
procedimentos
Algoritmo "semnome"
//


Var
   // Seção de Declarações das variáveis
   vagas: vetor [1..10,1..2] de inteiro
   x,y,op: inteiro

procedimento impressao()

inicio

   escreval("LADO 1")
   escreval("| 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10|")
   escreval("-----------------------------------------")
   escreva("|")
   para x de 1 ate 10 faca
      se vagas[x, 1] = 0 entao
         escreva("   |")
      senao
         escreva(" X |")
      fimse
   fimpara

   escreval
   escreval
   escreval
   escreval(" ###################")
   escreval(" ###################")
   escreval(" ###             ###")
   escreval(" ### RESTAURANTE ###")
   escreval(" ###             ###")
   escreval(" ###################")
   escreval(" ###################")
   escreval
   escreval
   escreval

   escreval("LADO 2")
   escreval("| 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10|")
   escreval("-----------------------------------------")
   escreva("|")
   para x de 1 ate 10 faca
      se vagas[x, 2] = 0 entao
         escreva("   |")
      senao
         escreva(" X |")
      fimse
   fimpara
   escreval
   escreval

fimprocedimento { impressao}

procedimento menu() {inicio 2do procedimento}
inicio
   op:=9
   enquanto op <> 0 faca



       impressao()


      escreval(" escolha ")
      escreval(" 1 Ocupar Vaga")
      escreval(" 2 Desocupar ")
      Escreval(" 0 Sair")


      leia (op)
      escolha(op)


      caso 1 {// ocupar vaga }
         escreva(" Qual lado? ")
         leia (x)
         escreval(" Qual vaga? ")
         leia (y)
         vagas[y,x] <-1

      caso 2 {// desocupar vaga}
         escreval(" qual lado? ")
         leia (x)
         escreval (" Qual vaga ? ")
         leia (y)
         vagas[y,x] <-0




      fimescolha

   fimenquanto


fimprocedimento {2do fimprocedimento}



Inicio

   menu()







Fimalgoritmo
